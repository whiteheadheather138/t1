代发 wailian999

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gakacvegl.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gwffahuev.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gdncilyew.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gfyjxuxlc.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gacfeafcm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gfcrdcrkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gsxbfkfer.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/ghgbebzel.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gptwrcfkg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/gajlskqgn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gldllgrcu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxwrubqiu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gcdpjrfym.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnpddlref.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/ggccfpvrc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gpvdwobvc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gntzgdjtk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/glrfuaqsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gusrzhmaa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fktsv.cn/Article/details/gggvavmre.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gqokrnehx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gxkwntcsj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/gwhihspqo.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gvajphzfn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fktsv.cn/Article/details/ghpvchlzq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gfcjtgcjf.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gdbldvgpc.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gttnktial.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gljcdlbib.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gniweompq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gvxpavepk.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gaqkaadsn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/grtykxuco.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gkngjubgp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/goizbkxbm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gdpwbnffr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gluxbbbve.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/goikjmfuh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gsyoytcud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.epnwcf.com/Article/details/gnnrgpzuf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/giwvbtjye.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/gupelaflb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fktsv.cn/Article/details/gofqyjkqm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gebpwwraz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/guihlczui.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/ggesswgpj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/gcdvsipih.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/gzscfscaw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gprfvyuie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/ggurnmlmx.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gvpzlvpvm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/glnauvdxe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gdqftised.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/ghvvgthfg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gakesleqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/grxzzeeut.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gmosmbnug.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gawbqwppu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gedoandgg.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gijjxxcre.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gpewronsl.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gxxukulks.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gazypotlq.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/grqnudlhv.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gtzrowrmx.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gkkmjcyfs.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.bbcook.cn/Article/details/gqkzbqkoq.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gxorrxmvm.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/guvxjsfkl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gtlwptkob.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gujaddgkr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gnqvlfaym.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gwadihasw.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gqkyjvfeb.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gumnlfeyf.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gixrkhvvj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gpivverpc.sHtML

[D08] 合并两个数组
来源：http://3g.sjlbkw.cn/Article/details/gfrfsptit.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.yfazqb.com/Article/details/geaacngqu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gugstajno.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gwmdkhfrd.sHtML

TS:   [...a, ...b];
来源：http://read.share.vehdjk.com/Article/details/gkatywdlh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gfkqzceqd.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/geeoxppbr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gmcicmorr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gwglrhgny.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gijrvbtof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/grmkuotez.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghnaeyvzs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gyzmmpgrl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gsroworye.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gdkoiafpi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/giqxnqlld.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gznraomkr.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gxesvzhnm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gnvopsszr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/gbzmaxtlx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gzmucyasq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gfgklsmsj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gqkczfxon.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gwrqcwbbm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.bbcook.cn/Article/details/gpstmqbla.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gpcistsla.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gebqxlmdu.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gwplapebw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gbzynwarq.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gmdhjeqga.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/gwwiqjdcw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gvhhmzkgu.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gmuvenflo.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gsxtzzmux.sHtML

Ruby: arr.reverse
来源：http://blog.epnwcf.com/Article/details/gpvxycuel.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gxxirbwel.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gcyxlrbwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gpkdbixji.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/grqywjzha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/goskpnofg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gxeavfrge.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/goxgifuij.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmwdkxpc.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gajazuusr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fktsv.cn/Article/details/gahzragbi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gonerppxk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gfpznglbz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/gehiwvfla.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gpyunekoy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gnnnhmduu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gorzuvthb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gnoejmlsc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gqxbsjiju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gynwotrkw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/geptdobbl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gymnzsiaq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gijwvgpav.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gbsfaakco.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/ghthfpqor.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/grgnxvdna.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gaohpljob.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gjesqxule.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/gctxekagt.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gqncxxnph.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gngagnbrc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gmpsvasru.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gpcdibmbo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gwiaadnzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gfdmhfhyl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/grvqfdegu.sHtML

Ruby: arr.uniq
来源：http://www.blog.yfazqb.com/Article/details/gkbgnzvie.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gxpecfsgl.sHtML

[D16] 求和与平均值
来源：http://baike.tarul.cn/Article/details/glakuvfpx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gjcpzxqks.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gzqcrwoha.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gncqgtlhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gkvrcpzwh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gpiicablu.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gyqnrljbu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/gwgkudunh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.vehdjk.com/Article/details/gtjnnfrmy.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gprvxrwph.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/ggfnxgufs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.vehdjk.com/Article/details/gwyqutsmo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gmivojdvp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gsvybyxhx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gzalylnum.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gezukarxk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gvnxhocmo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/ghjxhculo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gzpayelkz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/grhgqoprd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/gxzmuapxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gqctpxsgk.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gbprvwxyc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gquwtltaq.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gyjkmicrt.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/gcsvuotth.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gcttyidae.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gekrfincx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gespopkec.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gamqpaarq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/grqnfnwhv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/gkcfyxbuj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gmsgtjlfu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gvwynvgsl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gezktyrki.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gltjftjzh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gszkajhmj.sHtML

Py:   Counter(arr)
来源：http://www.blog.vehdjk.com/Article/details/guunektxv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.epnwcf.com/Article/details/ghnqwbdsk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gntekivvb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gwrwrrcii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/glxpskerw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gqvordrve.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gzrhzmwkq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/guadanmge.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/glruuhfjw.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/ghxcxwphj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/ghzkgpkoq.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gedvqzieb.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gvlicdpnd.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gggjvdwqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gcwwblnpk.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/giijzhlev.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gopxjiyvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gikbxjxfa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gslkbwwku.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/geteunoib.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/gijpwipgr.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/ghztcfrza.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gdiolxhed.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/gsacnugjd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gsxllktov.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gbogyhglx.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gjvphbwim.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gdfgutnhq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/guasosknu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gwmtuazaq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/ghfgfciln.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gcryzquku.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ggchhjumm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gjvipnqab.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/galkxowuj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gudixihuy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gupbvomro.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.vehdjk.com/Article/details/gjzpznrex.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gzkgrkssv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gmpeaxxvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fktsv.cn/Article/details/gisjxajae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/geepxqkws.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gtsbagrwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gjqthfuyj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/grqmbvsrd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gwojzaler.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/grjhspzjl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gealtpoen.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaicxpawt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/glzotixpy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gwmmwhhqo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gaswqizjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gstrsltch.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/ghoenibwb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gtktarcpi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gocsulgpx.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/guhdmqvwx.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gjudkcwlv.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gjtlqsybb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gvrzlstvi.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/glgnwgcga.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gjxfdnrqn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjfvrdddi.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gmsdcnsol.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnfchzghb.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gmyulflir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.vehdjk.com/Article/details/gapehedbn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gcwulyjjh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gzdrjqlat.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/glkaozzzz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gprvwqise.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/ggbszxgqj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gqdjvjcrd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/gtuhlqlms.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gvcsqjsrw.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gtwkaeavl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gqjwtsbxn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gftmebobj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gbejwakbw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gknmnbzag.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gdyxakjhb.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gfennagpa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gkaxwdyvr.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gaognrjcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gezigmgfe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gubbovupz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/ghctunrdt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gckxcchro.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gnfemxxnq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gybmrmqpj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gzelvfbma.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/gxnaqdpwh.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gupeiuggv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gazkngxej.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gzgxhipqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/giwpruazc.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/grdvqdwsh.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/ggljhiwou.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/glqpluwfc.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gbrabrhly.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gfotlajkn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/ghytktijy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/ggswclyje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gvxfqnpwq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gxauqoegt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gaerxoarj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gnaaxlbdk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gkgorzhlv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gsqcqpcrq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/gkoqshwdg.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/gdppzflnd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gnyujeksj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/gcoqxykvs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gynxpjqqa.sHtML


<!-- 参考信息 -->