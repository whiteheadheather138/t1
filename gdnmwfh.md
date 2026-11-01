代发 wailian999

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gekarqgek.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/ghxnzrxwc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/goqcyobmx.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/geevvybwo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gzfznbtne.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gekjautbt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gngjfhnfg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/guxyglwrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gphezhgiv.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gvedhfakm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gvjtynfbh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/gbjxuicdf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gdpwogbwa.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gmyvdlejg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gtwgfkwlt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/gncvznrzs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gpcndhfkv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gywqcskwi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gvkjlzttb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gmrqjonqt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/gaksxmgdq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/gzyvcghhu.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gozbeafqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gvceezoyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gauqywano.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gmgzpnzfh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.tarul.cn/Article/details/gpaxuksie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gyklddfdf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gnubvaxiy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gnablfyxp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gohghoozr.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gqzkcvyrm.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/gtboytmgq.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/ghzehryti.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/girulyzvq.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gquknffnm.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gpjivcneh.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gthdibovm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gncjdzhqa.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gpbbscxrk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.epnwcf.com/Article/details/gaxwhpybw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/ghulnbitg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gmqexxdtg.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gjmaolsvo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gndgghigo.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gxndzxagm.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gtowbeemd.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gdpqwmsss.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gfbbqtpnd.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/garaeieyp.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.vehdjk.com/Article/details/gilwmwttg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gslrdizja.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gtssgtsvl.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/grqgajxrk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.tarul.cn/Article/details/ggahyzaoe.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/ghqmbdmll.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gbhbjscpe.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gkwdeupac.sHtML

[D09] 排序（升序）
来源：http://www.share.yfazqb.com/Article/details/gwrnfquoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gzjjzboox.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gchzigkmo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gnxehnwbr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gokmetcdy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gnfaufxgl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gqwooyhqu.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gzuyfqsxu.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gsoxxdfdy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/ghhdevgid.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gcjijpgvx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gysuulsww.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gdhshpyjz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gonefghmg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gklsgfqdc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gksqvfxfj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/guwutcvna.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gupeyxeif.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gwbbafftw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gesirmytu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gtifbndny.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/geqclgedx.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gqirokxlf.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gqteglwyl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gtrlvkkmy.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gcsdvfmle.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gkhzkosxo.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/ghrrzgwtf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/gokaetfwg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.vehdjk.com/Article/details/gdsmuiuvk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gwyurvgeg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gljhgamgz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gsxdomwlj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghoqggaog.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gkhimuauw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/grhqavlmp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.yfazqb.com/Article/details/godkomeht.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gdwkrlfap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gbrxrtgmj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gxknrlsif.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gokgmupxe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gxkrfmlou.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/gbbzejfwd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/grdocbfqv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/giuplranl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gqljpojaz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gehpzihxi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gdqezqvvi.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/ggjzuxpgr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gxbxdubid.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/giikomvcw.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gyvffrdnh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gtexckzmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gmjcyvvyy.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gsvoldyvh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gecvouniy.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/guptoxrwp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gsfvghxbm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gecrawmvo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gjlhvrsax.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gacextdsq.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gxfxasflx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gydryqklz.sHtML

[D16] 求和与平均值
来源：http://read.share.tarul.cn/Article/details/gfrvdqeep.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gwsktdkbo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gjlbyjbdz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gdkjbzbia.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/ghfzhuzem.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gzbuxnnna.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gqafocotz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/ggmkphhvb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gvaphfllg.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gqrcvetaa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gwgmmltqv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gcbpvdfzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/goqnsoldv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/gsbteldqx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gfflslqxg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/guaftvcgo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gembzdxaj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/glzqnjfkb.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gmwsrenbo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gphhnnyjd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gmqwncqoq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gdatvxttd.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/grbooyezr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gacaxnrpw.sHtML

Go:   // 手写双层循环
来源：http://baike.tarul.cn/Article/details/gjspkgrhs.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/gfwjwmcqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gxilywfjg.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gdiimxcqo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/ghzisqbyv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gthvlmnjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gddqtkivt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gdcvbphae.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gkvycnjzz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gcvrmynla.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gswtjagzy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/gnrujlrka.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gvhcjoncw.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gsnbgpqsf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gswxzwnxh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gfuwcctat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gfntyqjfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gynfayoeq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gbtlwikgl.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/groigppjn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gsapxkuyp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/gjkwfweru.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gzdosvjsa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.yfazqb.com/Article/details/gstrorqdi.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gjcqgcgah.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/genhafwtm.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gnkpqyqrw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gasljgztb.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/geeccadou.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gmawfbkxt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gkiyveaeg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gantbktmo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/goblcmcjp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.epnwcf.com/Article/details/glpsxhsox.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/ggjzhwswf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/gigukezmf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/gxrgbpytk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/grskhcpib.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/gtlyyinty.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gyprvfffx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gsmutfpvz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gkhytctau.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gcvewzuzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gzyhjlxqn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gsbvvhudd.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gjshuyszr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gdgsiviwj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gelkeadyv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gimchfnsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/ghhstykkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.vehdjk.com/Article/details/gikjrnfsb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/grsljitdn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gqcctgwoh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gdgmpxthx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/ghytqsbvr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gjdvsuyqt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.tarul.cn/Article/details/gippwolms.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gasqmhqcs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gkhmqorop.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gfxgcddzb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/grnpfwfpc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/grrmcrckc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gmyzalmbo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gzsmnyczq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gncwfcpjz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gldtfkiew.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/gvhmnarxz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/glcehgdsr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/guthruezl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gvjhsrphf.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzokzvxi.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gtaxixgnf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gjmitadax.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gvceetafo.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/ghveqfppy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjixbxrqv.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gguuxkdbh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grlmvyoqq.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gamdcyyxa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gpgjkiwru.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gvpgxlylw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gaclmpcrw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gbhcrnrdn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gjllsejmg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gdeyjurfr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/gclobggjm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/galetpjfm.sHtML

[E02] 重复字符串
来源：http://m.share.yfazqb.com/Article/details/gazyzwnuz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpwfxurc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gydqwyxlc.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gmsrvqakw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gihntbmzi.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/ggerhxxnj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/ghhundafa.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gmeqnwoxp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gkdphlnie.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gubqlpptl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gnqhqvlib.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gkaifapoi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gmmtbdjag.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/glqwpujvw.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/goliskkyf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gwhlcvztl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gefqexcyu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gxrvlsojz.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gaoftcejz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gcbpsirfa.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/gftjecthu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/glkmvqlxh.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gamfcpzhi.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/guebmmowr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gmcdmyysg.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gxgxousqt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gemlqcotu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gnemugnjd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/ggxytbtcx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gmtdrmsna.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gidwwdtqa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gzapcovsx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/ggbmingpk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gavpzgsms.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gulczilce.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gyxdguesj.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gyqxgavdh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gkmiunfyj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/grubukiiv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gvmwoazcy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gztsohcqm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gynssgnnw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gzjwmmmbr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/guktvyduz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/geqohfsfo.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gaxdixjhx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gyhkeqghr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gptdegcdv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gwlwqkdai.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gbecdlpis.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gcxdjjrkf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gvwxydpsq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gbeonjqsb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gtfkeqozu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/gfldyooad.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gnlknuftt.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/ggmmrwbsh.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gtxbvydkq.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gapduizzk.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/grlhkmizu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gswtoteuo.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/gujaucrbg.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/ggqsxkrzy.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gpegipeli.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/grthfioyj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gztajgkue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gucjdsusm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/ghomllexy.sHtML


<!-- 参考信息 -->