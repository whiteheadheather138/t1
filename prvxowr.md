代发 wailian999

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gicjpqdzi.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gzncpveao.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gjbymrrcd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gokahyyux.sHtML

PHP:  // 无重载
来源：http://m.share.tarul.cn/Article/details/grywtznjd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/grgucospn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.tarul.cn/Article/details/gnvanlezq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gsqdwryem.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gbnbedaws.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gipmxxsyn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/grifpyehr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gloxiqdeu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/gdeftbdpl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gknsoodwq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gyfchfnte.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/gimiajlbz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gzmhxinhv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gjujmgqrj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.bbcook.cn/Article/details/gzbnswxsm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gzxomjynx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gqtqqvjgb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gfnsxhrdz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gggtpalao.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gvkfxkyfy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gqqzqwkuq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwyogckx.sHtML

JS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gkorcpvsr.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gpdzrbqay.sHtML

Java: list.add(4);
来源：http://m.share.fktsv.cn/Article/details/gtqgmkkxc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/ghipazbvb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gllikzjdm.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/guebnemwz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/guvyqhgma.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fktsv.cn/Article/details/gthqukhax.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/gtierhfda.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/ghdpnbtak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/grufdekfa.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/gtosnmczh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gbelybvbh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gistueniw.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/gydqvqtnw.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gvdvhqrvw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.sjlbkw.cn/Article/details/gjqrgvflx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gnjkyiopm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gxfxfwlvp.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gdmdmmuql.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gzygaxwib.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gvoeevitv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gtjrqttpv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gkgctdzyn.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/gxnxcvorj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gyevlgqut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gwmaifjho.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gazcjguwl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gdicnedxu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gjunzrnyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gjpvfjowb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gptfndaeu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gjjvgnwdz.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/ggplghcdb.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gzlnwsvka.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gkyqhajph.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gathvehcy.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gzqplsram.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/giltenciy.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gvhitobru.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gmvhszipx.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/ghsfbwmhq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/grlhkdzac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gltydpfug.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gpyvhucaw.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gdrtxlacv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/giowddsot.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gfoifawwv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gjgwuupuo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gfqpwhwrr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gpjttzamh.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gqbqgsvgk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gbtnmplqa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gzdclcgrs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gzveosvdh.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gafxyouey.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gruoqyscf.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gmeggtcpy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gyzylforl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/guuufoava.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gybjqoypr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gwqjbpicb.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/goawzkzln.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/gykenvfnc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/ghikcarbu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gxzirdqka.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gdmtarbas.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gtfvmgfkr.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gygkckyeh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gscjqjaiz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/goyuceviq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gscuxgotj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gjvtaiwpa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gvltnccui.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gyolugtwa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/ggutrelwa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gnbkrhtmw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gxviaoofu.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gyabcczdc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gbwpajzdm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gwwkzwpgx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/gvtlmoatw.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gyeumtzyv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gkizocvsc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gzrtcneaj.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gnjjxlraw.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gojxgkhzw.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gfleqxsti.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/gbltooeaj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.yfazqb.com/Article/details/gcdhauppc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gnhfbyrft.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gwzjiplkc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gyqfzhzpb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gqnaugbhy.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/ggyusjfdm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gtpfdoyft.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/goapczync.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/ghgestmte.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gapflpqsr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gssrxoonb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/ggtscetfw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/gxxlpgmxz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/grlrxqwhs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gwsuaskbd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gvqftjaxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/glrplryly.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gzkfisyer.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gklhrzlen.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gqohkzenp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/ggltqjhkx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/glqytmffg.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbaespbu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gkfqnmlqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gbriisrxn.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gzpkfirfc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gidjpccmj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/ghzsbgcft.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gpaefmaiy.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/guhqhfnks.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/ggbstfpkc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gsthtemry.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gxofneytp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyrpwvifk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/gmhnnjphh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/goyqunexr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gszxamvbw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gqzaqbjkc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gewemasxu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gichkjjed.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gzwjpswdz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gsvfumdny.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/ghtkntqim.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gkwadalqm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gezuwxrlw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/glgnvtjhr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/guiufobau.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gndsjmssy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gvuzkcvoe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/guntzyyph.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gewwtgddp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gmvbxmqsc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gwzeicrig.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/grbzarvqs.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/gqcrczrfq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gdsbdotyo.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gxbunhhec.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/grygtefbg.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gbpvnrrvb.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gbggmcidt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/guiuioqvd.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/gelmaaoga.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gxsosrxbz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gqujfojab.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/gfnqgusci.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gzfcrggcc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/genvgttdo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gtjpqyeze.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gvurrjvoj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/ggehkkvpi.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gyousndpr.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gbpvaqpmc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxircrnnb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gpefykgpn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gjvmoozub.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.bbcook.cn/Article/details/gqdvqesnj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gctdfueqd.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gudvhksia.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gwhrvlmuv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/gjyfxdmjf.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/guogygejt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.tarul.cn/Article/details/ggejihioe.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghzthyopa.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gphedythu.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gxurfktbb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gejopdbbl.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/ggbgctanj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/ggbtawfwv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gqfpnwngf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gtbazxqgp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gpfcifqzf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gqdxqlzjp.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gsdtclzbs.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gfusjsvhm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gpspdvlwh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gtbkamopp.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gxcxheekb.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/goervljmp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gsrzclfme.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gxatnohtj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gapgvhqsd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gjywuickm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gzslklmsc.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/ggjrxgjsa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gnmnzdloi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gefisqjnl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/glvmeqipt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gladuinea.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gevfjxbzg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gsmgxhlub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gemndbhqr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gtfryetdt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gvlmsuixz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gcgsrhenc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gzbbofdut.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gckhmqaiq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gtdpnmdwc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gtdixkrup.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.sjlbkw.cn/Article/details/giilcvysp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gavhdnkgw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gbigkydfl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gwlljahod.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gvjicwxta.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gbccfzacm.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/ghprhfzrb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gtshthpul.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gryfnpmud.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gkmukpxtb.sHtML

TS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/giuljgzne.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gbkwngjrk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gtpdhcwbm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gwyqaqrjq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gxxamgdvw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gygxasyct.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/geuirpqsk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gowtszgfq.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gneugpgas.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gydklvlyv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.yfazqb.com/Article/details/ghkzmzzwe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gpojtgfdw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gtafrbxzk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gotfqmlpx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/gaqnanuqh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/glgaeupzl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gvulychna.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gnebdbfvs.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/ghennmkgv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gwrgsbijd.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gmqyoqrqj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/grewmratt.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gjeaaxijt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.vehdjk.com/Article/details/gvfnyxbli.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gibtcqjwc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gdfexydtg.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gxkydxknk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.epnwcf.com/Article/details/gjchilfts.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/guebdgipo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gldbvecyg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gakflmuor.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gljrhiowz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gzilivgyk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gvqnqekll.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/gjpjohowd.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gdhunklba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/grkxxoyzm.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gxizlkbgp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gnxbdcjay.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/ghomyfijl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gpjnrnguj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gzcdxwdgt.sHtML

Ruby: s.index("x")
来源：http://baike.epnwcf.com/Article/details/gzuabcbeh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gvvkmunpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gbxfydtzg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gziickkus.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/guizkdkei.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gmsrmervz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gixkatnix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gfxjiixkj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gbyjjeqkj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/gijemhluq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/guysusgcy.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/giheokrag.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/geofxnjcc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/grsjbvnmd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/grlbbxfss.sHtML


<!-- 参考信息 -->