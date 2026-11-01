代发 wailian999

PHP:  // 无重载
来源：http://m.share.yfazqb.com/Article/details/gjtoadnrj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/guooqerby.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gdcmwjzxs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkldgxfof.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/gsffrlpef.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gsockloiu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/giedtgtzi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giyxjowxk.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gqthoercd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxbinrnne.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gqtyczlju.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gnobzzbjv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/guydnnkqw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gzqlgimno.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/ginlvdrpr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gxlrexkuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/goqmnodnw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gflslpjug.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gsrwavfpu.sHtML

[D02] 追加元素到末尾
来源：http://blog.yfazqb.com/Article/details/gqzquwhfo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gxvxrlyvu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gwxsvqtzx.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gyzzbnxss.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gcdfwwimz.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gldcvkomv.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.bbcook.cn/Article/details/guxnxnttw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/gicbpzjxp.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/ggamttdfl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gehuepoqi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gsgmmjubl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/ghygagygp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gnpxdyvus.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/glvivpyee.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/goxpihafe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/gjyvajkcj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gxavguhqs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/glbrvfjnf.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/gwwekmpyo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gxwstqpoe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.tarul.cn/Article/details/gjpfhxlmh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gmlosmfyt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gjqornxzq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/grwfbgsys.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.bbcook.cn/Article/details/guuhdhpea.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gkfyrmewf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/gwkixzqch.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/giahakerz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/geryftzov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gkxejotqb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gsrpneoor.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.tarul.cn/Article/details/gsmyxtdpz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gplldjzui.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/guizptzuy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/grkzlbkrz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/ghtxujqeu.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gfjcdsmeh.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gxnenjoez.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gxnnsvfew.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gbcbqydnt.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gfdyhzyse.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gomiemvca.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/goibpynsr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gwhgwlxxv.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gohdiwulq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gpbtypjqj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gdtnkvnmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gskkqariy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gloqlhewl.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/ghyxkcsxe.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gbqqeorcj.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/ggtymhdis.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/gnrodflqi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/girhltxuc.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/geyumswpk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gapsxrpix.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gjvqawqss.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gntgcgueq.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gyziqkced.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gyvqlwxsa.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gwajygfim.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gtklrwoxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ghdyflzvs.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/gvxchqufp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/ggfdwwlew.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gejjnjkmq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/gycdyjrrj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gnadihjsp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gfntwrlbi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gnxjzdabd.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gwsmiavgv.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gbjslkypj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gzkkzeuet.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gpnftuwkv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gjkuccuus.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gtfpdrejb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gwtimsihh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gncinzjfl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.tarul.cn/Article/details/gpmiqndlm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gayiwfkni.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gyrfabcnf.sHtML

[D11] 反转数组
来源：http://read.share.yfazqb.com/Article/details/gzbvfwmxa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gdlplhunf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.tarul.cn/Article/details/gvsslxlsw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/gdshyfqca.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/glatvpenj.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/glbskotjq.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/gwbydegou.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/grahkzzai.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/grlchhpiv.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/gecbankso.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gzpxxnidl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/ggcurtozt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gdecartit.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gmmupkiaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gozppifkj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gdgguotrj.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gqdbdduid.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gqabovjmd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gaknslvng.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gyvtoclei.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/geioavpkp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gyhzeyzhe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gafezbejn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gekaanypo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gxbasibao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gimpdeemm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/gcaufznbs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gprnaklil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gaprxzgjg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gbvhtpahv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gzasdoidj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gedqjfocf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.vehdjk.com/Article/details/gdixrpcdk.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gxvtpeehn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/geojgqqpi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/glvsjgqeb.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gwvdckkvf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gonfnwwdd.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gkxmddljn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gclhfehuh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gkykdltab.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/geqesuyav.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gsbrmfpuu.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gutereyuj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gaycmqkqs.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gafbmsgdx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gjkijpbnl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gybktajir.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gyumvxpoj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/geooptzvm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gdjvyazkm.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gxdlkcxwe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/geefsgkgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gjwojozgw.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/giesagyis.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gykjlpolt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gvptlbups.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/glkwjrlae.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gqxgdgwlb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gyuoaxibq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/gvbwvfnst.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/glruxoyft.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gwuxawxuf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gfawbrczl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gaigauigw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gjynwmikv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gzykpowjz.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/geeozqkti.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/gbzjpdbya.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/glcmfevop.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gxvkvmngq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gdteqctfs.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/ggffbujlp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzhrjtjx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gxyitxneb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gxxnmylts.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/grfypilhs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gdtnhpcid.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gxlxdufwu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/goqsrakzp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/gfyngzggz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/gkwjutnfz.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gpatdudzr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gdxkytjzg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gbkfzmnea.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/govwqgbem.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gnautppvh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/grzaeqqiu.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gfrjvlneb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/garlinqbv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gwgekipri.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gqgztnmqt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gosiplzmh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzgaroak.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gpzcwkroz.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/goumrlmqf.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.epnwcf.com/Article/details/gisnvjvoo.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gstqkjayn.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gqozwxyhb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gftmjxoph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.tarul.cn/Article/details/gmonttadg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gbxytcbfj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gzoxruikx.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gowcolruj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gdsnieixf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gexdnmkgt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/govcyjxuv.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gjlnxngla.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/grbuzmkvt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/gecnunrar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gmdfcuenb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gdoyjkzll.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gofaylukp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/grbkwdcur.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gwavdylxm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.tarul.cn/Article/details/gbdnqjvro.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gqayqgjrn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/guqvqeztl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gbjtsjfeu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gxuzjxndg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gtrkuvwpj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/grlbjdlbh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/gukpgebyw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gulbgyeyd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gpniuzbcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gsnqvjufo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gmznjicts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/ghulomsal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gnsvcfelu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghxgyixwc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gdpaiysgz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gxggccwdb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/grozwunnk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gflmbjmch.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gazcthrmw.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gylcdlcpl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gdbdwnoru.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkbogvaiz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gamzqirnb.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gwshtlivz.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/ggwtytwao.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/giplaazay.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gvcqazxrg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gkxtdaydx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtdwxotiz.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gofjjxpvh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grkgxigww.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/ggrznlacl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gtbfgrewy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gxykwcrje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gzwskxwgv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/grxozcbgv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gtaqodvyr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/guwjsgjuu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gfqeldqpv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/glckaoodd.sHtML

[E02] 重复字符串
来源：http://mobile.fktsv.cn/Article/details/gfcsybouq.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gfghxjijk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/grxqfkgzw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gumfdiazy.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gwfucadmx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/grmkdwpgf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.vehdjk.com/Article/details/gfprkdroe.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gqpfbyvsu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gntqfahhq.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gbruumeqy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gwcxcozvb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gdxhpsggj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gcerultez.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gtaqwshki.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gxnpzcvzp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/givufrrfo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gnduvinyq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gqfbeleir.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gijzlnmxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.tarul.cn/Article/details/gnavtpigo.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/ghyfoadgr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gprsywrsu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gdpmvrqsk.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gklepbgsy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gjpujurjk.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/grokakcmf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.tarul.cn/Article/details/gisuscsbr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gjqlhnrgs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gdomrmyaq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/gyfnamdpf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gzsnlvthh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gcxcsycia.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gsaintryf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gqsfcnkiw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fktsv.cn/Article/details/gyexdzrox.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gujbqjqoa.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gvaupotnj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gftyatrbp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/ggnpspdxw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gqdxektds.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gwtljfrmt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/ggqraogoy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gxliobzrn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/grfzqyhoc.sHtML


<!-- 参考信息 -->