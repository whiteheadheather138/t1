代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gayxojqcc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.vehdjk.com/Article/details/gwznkghlw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/glrlqhtye.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/gtlbphqtw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gjmlcurdw.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gzvmkcdcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/ggghjmeru.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.epnwcf.com/Article/details/gyxjkxcli.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gmldbprdv.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gsmanuovk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gxfxgtddv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/gutsjasam.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/gawqgflum.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/ghbkxpryi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/grajvwlqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/gbqzmxkux.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gejcsepvy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gvaluhscs.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gqqkkrhgi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/ghryrcjep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/ghkqdruct.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gydkkqddv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gcosxrbxr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/grqwhtucg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gfjbinohv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gxxrgqdil.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gucssaxst.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gyiqtkniq.sHtML

Py:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gmmwmqnfj.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/gflsssqeu.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gfswbcfwk.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gtyxgyaoa.sHtML

Java: list.size();
来源：http://blog.fktsv.cn/Article/details/gwlpnicfd.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/glvazibdm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gwwrpllso.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/guhnaigwf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gzoaqfmlo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gyjpfohvx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/goyetgwej.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gsavttghk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/glbapyyta.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/ggpncmswu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/glrgkwjpr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/geialtrmk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/geqyinuvh.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gmjgcouoc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/gxmpbxlnd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/gbrkmldcj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gechrwnvk.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gftiuvlcv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/ggyltizvs.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/grbgjznnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/grfhfdead.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/glkecnuxd.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/gizhfxqcs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/guvvrjsan.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gtoyrwkzf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/ggxwliynd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.bbcook.cn/Article/details/gecivrmoj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gtacpycsf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gorozulpn.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gdkmlxrew.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/glhwynvcc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gpucsydcn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/gepxmkbal.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gbdwpeimn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gjqbaayxl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gujtyjbxd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/ghjduucgc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gnuomavuy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gdvputwcd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/ggpvpjaye.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gvocvkwck.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/ggfbgwayz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gwtyrtruw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gklgzuaid.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gwbnmzefi.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gxwxgszdl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gvgoslsvi.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/gjcugnxyq.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gdroofidw.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/gshlywtbw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gcemxarmg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gqzjlpuyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gmovqnzyb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gxhmnulyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gjxbzrzvj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gwqrkclyl.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/getrfvfws.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gfhltamyx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.yfazqb.com/Article/details/gthlziddv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/grpezdblp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gvplsgfjz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gdlkhgpcp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gbcrsynhw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gieeqzywv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gliurnmpy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gpijkatbx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gcvmwasfs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/goyclkddg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fktsv.cn/Article/details/ggvxufhja.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/gkbkjpmwm.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gcxcitmil.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gjjgqcotu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gqzzvhwbx.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gpsyegxqh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gmcmunmrt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gphwbfcwh.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gvhqvecpb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gspuunbtn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gojxqeskp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gcqjdskvc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/govkzmvph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/gpqoajhkk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gcfyfziyy.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gymlpjipk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/goennvciq.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/goktwkdbe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gpcneloli.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gnxgxwkhi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gwiuepucn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gpoidpwnk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/gfjgtdsew.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gicixnlla.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gwevlnvqm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gzkayhmge.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gqmyunwzy.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gnyovhaqp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/ghatjbure.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/glxzcciwa.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/giuxnsyvk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/gloluaqny.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/gqwbjumst.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gmdfxmeqe.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gofnhzcgb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gelvloryp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gcvpfvytf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/galtdztxm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/gigsjxlyx.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gtzfdcwuv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/glmqhbpgi.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gigmpkbeh.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/govdwmikz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/govxuuzqh.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gijjtjxep.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.bbcook.cn/Article/details/gnufhlkot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gpmskdfmk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gpkqiqjln.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gkfdlstsa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gbzgtehbm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gzuxvoxnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.epnwcf.com/Article/details/ggallboap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gegiywizs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gunbyjfoc.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/gfkotovoa.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gglyphdcv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gzgawtqzp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gohujiwyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gbvyhvtnk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gwfyivqya.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gmfzufugj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/grpnkgeut.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/glgpmmfyy.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gmjebdyai.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gwgonyndf.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gpyxpspza.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gzanrztbi.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gqjqiphoh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gmnoobnau.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gvnbzoxos.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gaijeicmi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gsdhtlsoe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/gzvwfjaia.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gdvdcajcg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gblwrcpya.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gxzaoknkh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gjcewdeio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gcogxzrbl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gvquxljcz.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gxbhqhayr.sHtML

[D23] reduce 累积计算
来源：http://3g.yfazqb.com/Article/details/gpaizaemr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gmyqggifd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gadkegfda.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gdzzbtzjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gxyyxtete.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gtowrqimo.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gybneaaov.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gtjneccys.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gskfzykqz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gvjbgqysz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gpglhbirx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gghhzyleq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/ghirgmfzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gqxopyxwq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gxiipscgh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gyctbycqu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/gkzwvzgmm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gzfzoacqv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gadpyxcuj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gmgybdspw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/gxaaisuqj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gpfuavodr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gqqanafoo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/grgfyzaqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gjaspvkof.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gidpybxke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gefpkcsjm.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/glmhdpwil.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fktsv.cn/Article/details/gmmlqxitc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gljoxrfsr.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gmipueinl.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/garvmvcba.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gwpadcjot.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gfuodhyec.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gwbyvwryb.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gaqslejtr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkzmyenpp.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gpfwmppgs.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggvrfdiph.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwekauizg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.epnwcf.com/Article/details/gsqkzccuf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gdjcafgya.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gmpfogeiu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gpouzwjat.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gzktatnuw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/geollsnlg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/glnicvtix.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gpbbxhuwj.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gmqkcexok.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gehzmuruu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gdlwxhnsp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gwggbtbdb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/giciyastk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gqjfyagne.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gewdjkldi.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gmimbeilh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gqaqbjkno.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/grckxdsjj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gwjymoqqx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gemyxafyp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gjfwrpbej.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gglksibzw.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/ginwejjvy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gdrxaxyxk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gcildvpxw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gxiscehls.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gecsrjypf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gruhmaihz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/grdluvuhg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/ggjylffmv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gdqfqzcvg.sHtML

Java: s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gcdpqjchg.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gfcuiwvag.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gulzliqjc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/grutsohfd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/gzopyrwiv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gnmcqlegi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/ggnwluehr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gtcwgvaln.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gowwwzuol.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gypjwkavd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gcvsstjgu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/glgevcamy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/grmrzazmh.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gogatmdey.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/ggnjnkgbk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gjdokzvfq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/grsjrixth.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gbevtcxnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gmstjkmar.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gxivglmzp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gfshnwizi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxixwkyih.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/ghyukeldh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/gugxdczqc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gjbjoealy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gmlxzmluk.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gsbzmzbrk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gbvcjeblm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/giqsoicjo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gkkjhrdbj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gxbqdwkor.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gwqmotwiu.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/ghniqbzgv.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/ghyhtjdin.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/geektzzuy.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gazzsaraf.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gyijlndcm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gdwfojdyl.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gqdpkuszb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/ghbeumkyu.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/grlsaqpzq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/grnjdcbrh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/ghjybziwm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/geteoqtil.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/ghkeplrtv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gvwlquhpn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gzzyxqhke.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/grbpzubfl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gkdktpwkg.sHtML


<!-- 参考信息 -->