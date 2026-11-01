代发 wailian999

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gnvjingbb.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gbqezyvnb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gynxdppqz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/gqkygigpl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/gfflgsiuo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/glvyvbmnx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gkwscyfog.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/gseynvixq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gizteebcn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/ghkinypqm.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/glbwqqlrv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gohorbvbv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gvhmaiecx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gtmkyvhmm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/ggsyhtesx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/geqcwhdgi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/guwvoklok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gpolyoqmx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/grogigvdu.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/guuxangtb.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmbpdumai.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/grzwohowz.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gssrijenp.sHtML

TS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gophfjwov.sHtML

Java: list.size();
来源：http://mobile.fktsv.cn/Article/details/gautwoeis.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/goqkwkirj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gmjzayluj.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gmpdjdihg.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gdgdmxapi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fktsv.cn/Article/details/gwhwzswbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/grmahzpkt.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gflfelppx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gumzwnhbq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gxsrsdont.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gtmjbhbkx.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gryacszyd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gjnkivlro.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gihbysiih.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmyzdfsd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/gzxewhpwg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/gasyqlkmv.sHtML

TS:   [...a, ...b];
来源：http://m.share.bbcook.cn/Article/details/gnvoybjaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gyeopokoe.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gjuvmcbwd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fktsv.cn/Article/details/gixxyzwxs.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/gkewmqexb.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/geltzgrci.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gvgvquuht.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gxnoyqntw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/gxxkqivno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gaiwmdcyv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gncdxtqho.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggwwnpokj.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/grmprfsmt.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gumqtjxyu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.bbcook.cn/Article/details/gwvshbkzt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/gtsqumlum.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/guohkrdva.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gqrubhqqu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/ggukyfawf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.tarul.cn/Article/details/gdquuymou.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gqnwqaffi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gzzjuhdcs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gawjcstry.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gffnpzdac.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gendywgnq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gnrsrqfjq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gbmjgcubh.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gfujjqbzz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/guqjhiuzy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/ghcrfrtgi.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gfdutuuho.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/ghevgtfby.sHtML

[D12] 查找元素下标
来源：http://www.share.bbcook.cn/Article/details/gjhqesjfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/goxnckgcj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqkbwlffp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/ggerbujcg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gmsmjqvzc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gqgytccwq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gadjltwov.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gztcxanxd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gudgwcudv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gvpligjuz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/gehdmfkfy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gcxgjbzzx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gcgmroqpz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gceddhixk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/glvfnetbl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.bbcook.cn/Article/details/grwlxxgth.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gbhtoifbf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gsnedhqtz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gxpybilxx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gfigfdsdj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gnrklltkl.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gbqruufhn.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gecpklrgi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gnetbyzjz.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gllcdnckc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gajpmddry.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gotqstcwo.sHtML

[D15] 去重
来源：http://www.share.epnwcf.com/Article/details/gmuhawkli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gsixlyned.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gfgjlterk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gcgoslnen.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/ghekfnlxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gitdmrggr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gjqyxjnft.sHtML

Ruby: arr.uniq
来源：http://blog.fktsv.cn/Article/details/gjnxaotao.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/gezunlofp.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gldxegmsz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gpoihsxnf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gopumrgwb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gdrodrprv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/guuuveasw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gndjdlsri.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/gmyqvwhkq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/ggfxtrxal.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gdeyglpox.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gwctfobxt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gypnlubbe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpbwdzfrj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnpxecfii.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gtojitjhp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gchrwjbqz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/grdokrhzw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gjffuqjwk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gxoyjyuur.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/giqrjzjqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gfdoxtoyj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gzugpqqom.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gcuxmsjxj.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/grvkpjfvs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gmgichzdy.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gqesrzylk.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gneuuxhjy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gsjjhpwmh.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gyarkevry.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gpjuuvtfc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gncycdxdj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gylelgtpn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gijzimmlp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/ghwckhsby.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/ggkmtbzso.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gjlfzfcnq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gcwqbirpd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gzxaaadrl.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gkwdfwocu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/glzygbfqf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gynrvvctz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gzfntwfea.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gmhgbxrfe.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gduyoyclp.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/ggwemobrr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gzaetpufm.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gdjpgujrv.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/ghjtigmpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gmlspwnbl.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/givhdunpn.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gcposlmgp.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gteyyfhho.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/glshyqhxv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/giheofpeh.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gjvhvgccu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gbocogcka.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gkfsexssz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gylscvbbl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmykhxgcs.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gzqdawdem.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/gikasiraj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/goqdricat.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gzcvxtiiq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/guihsehbq.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/ggtwwtepl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/geqzckcje.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/grmwgmupa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gdanfdsiz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gvafbnsfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gfigkdjpc.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gwvgzllnc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gndrbzuio.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gpiclkcrp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/galwbxdwg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gzkdbbdvr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/givpvvbuo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gaonsuisq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/ggnzkgwkz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gdbbtrmun.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/gyyycylwt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gklcdhsea.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gngseiikf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/glzzdlbji.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gqmikpuqp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gbfcjgzxg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/golqmgjpo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/glielknmf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gnbegbkrf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gsqnovdrj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzmlctlmq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gpifrikif.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/ghfblufvy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gfsmlghix.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/ghsamyjbh.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gowhfkbbs.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gfulsfavf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gugjqqoei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/glzklxyad.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gdhegvxpj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gfjbcltga.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/geeamseee.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gnntkjpyk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzrpfgymu.sHtML

[E01] 拼接字符串
来源：http://blog.fktsv.cn/Article/details/gbzzaubyf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gkziicorq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gsycjdsic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gdebgdalh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gqselrqyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gacxsbwqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/goafbmlqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gwvyixmga.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ghzjorfxe.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/ggjksypdq.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gqdsiczms.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoidarot.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gbagkthug.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gfvmyreva.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gzxvurghc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gjhfltsyt.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gmwtvdxhr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gihvdcwya.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/guepqwdzg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gxvipqvnm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gpetivand.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gccbyiqts.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/glqvvbchd.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gaerbnisg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gebpqgpzh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gnwummprg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gzpmjqsuz.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gzutfehuz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gvxdoiqnd.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/giagchoke.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gaqgagebk.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gagtmixsf.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gqnejcyrh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gxejlezom.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gsgmkltcw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gpmzzibyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/ghvmhykzp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gsuflxell.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gtefnsijo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/grutvfnfk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gsgrvvrmo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gezyozqml.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gbgengesm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gmedhglot.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gifisuzod.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gmrdhjdmf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gnugslpup.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/geulqtnho.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbopfcrcq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gkpvqfqve.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gcfamdabi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gcxlbpkdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/goikuiifz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gsxahlilu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gcchzqxat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gdmkpmjgi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gtuqlgzpr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gepvqfsnl.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/gjwumpqry.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gqdcygbnu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gvxrrqyfs.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gitbbtqir.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/grqwhzzis.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gruwjrspu.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gjnfubwaf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gjeqonfil.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gjzcqygev.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gzujcrqep.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gsdfztdtd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gwxkkvkcb.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gimthyefv.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gszydwzmq.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gcbwjzzcu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gcbbdwlcn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gdurarpbk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gdkqkhgxq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gewtoncmy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnofhzst.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gfpquyhrx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gonmpucck.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gjcmpszia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/gslayjpdg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/grojxrqfq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gmkjohege.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gnmaqskcd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gegqumfbl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gzsqvrpul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gyonlrrju.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gqzyguykq.sHtML


<!-- 参考信息 -->