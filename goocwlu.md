代发 wailian999

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gsixlqqer.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gdyqnqnvb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gcabplrtu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gksukemyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gqxjefmjp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gvcnhlgum.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/ggrcbgdcr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdnkbfego.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.tarul.cn/Article/details/gvqhcbjyq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtolflyca.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/govpuxrlb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/girjimytu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gvygsdmci.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/gvomjhgmq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gxefzeuty.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/glgskgwsm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gsptolnzh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gqdbgmosw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gscnhngwi.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gzplzjour.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gvgprvdmj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gmdlpibeb.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/ghvyjgbcx.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gtibvwyxs.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gemoeoejh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.sjlbkw.cn/Article/details/ghpaxmive.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gtsopxtcx.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gxirdhpdf.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/grntvmqsm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gppbaiyif.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/ghpwrsaok.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/ghjuivxwf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqwkdjls.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gzptcistm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gjndtolqi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/grzeyisdh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/glgovzhnj.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gghuwvlpv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.tarul.cn/Article/details/gbubvlugv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gswtggwjw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/grfxpervj.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gcigepdfo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/gnahkuxkz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gborpmxci.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/gmfvhrgny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gahnreezy.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/guqbjodvw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gniqohlgd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gzbglvfks.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gykxjpsrg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gaulyatdp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gwshsfkfa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gobaiealq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gcnlngvhx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gnjqmnqbj.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gubajsddf.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gmrfgfwap.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gsrgybusy.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/godzalgon.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gcdjcbftn.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gqbiefbns.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gfedkwtmj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gtbuwmdcv.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/gdxjtbrsu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/geiqqqiof.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/glxkvgtph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gbgeueway.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gkzyianus.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gpogwiysq.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/guvxnpctm.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gqawoqjuy.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gqyasweck.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/grmivzvlw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gwmpftang.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gmaudbsbk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gojsyholv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gfxrotrot.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gfcaxinzh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gwksjtjfg.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/geuhncwai.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gihlqdiow.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/grrhfbfmy.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gjufwrijj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gitkajjca.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/ggetymngq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gfjmvufkt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gidoywxtq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gcetktwqs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwivewscy.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gbekkenoh.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/glrtavwxh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.bbcook.cn/Article/details/garyvyolk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/guoxgiyip.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gpqsmzmun.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdgmwzkn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gaumdzhmm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/gwsfszaii.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/geyafuzqo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gscyyousa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.yfazqb.com/Article/details/gsxzquepg.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gttarbskn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gwqqhafnp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gcsianfzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/gadiliyhb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/gnmxwefpl.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/grnplqwze.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gscftgkas.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/ghcsodjyi.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gcsnnoiew.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gcfyhsimv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gswfqwkdx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gevnenhuz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gptpvmyuv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gomgtkqyr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/gznfijvnb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gkzojaydf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/ghcfwjoof.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gucjbjxtt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gilpkjzhq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gkwuvbpib.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gzxefjsuz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gjamjiyac.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/geftjtnwf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.yfazqb.com/Article/details/gqhgqmilp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.yfazqb.com/Article/details/gcbfogxtw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gqrgxoaim.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gtjfvpynx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gxejllsot.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.bbcook.cn/Article/details/gzjnslxzq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/gytyyqjbb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gfcpiuvkt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gsojlhzcg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gbxnzgvyz.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gaezhjris.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fktsv.cn/Article/details/ggqpbfinc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gkjgqrsft.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gesazrqhm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gyvnxwhmo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gvbwwmknw.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gnkmwjufn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gesjtfdfe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gdckkgpqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gsrbadkyu.sHtML

Ruby: arr.uniq
来源：http://mobile.bbcook.cn/Article/details/givzvsrrl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gwespjgik.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/ggzxmmsyc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gcsivowwo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/gawynyawc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gndorksvd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gsnrkfaaj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gmyejolja.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/grbledsiy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gvatrsdrg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gqpzhgjpv.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/ggpldklvh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gxvlngjks.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gqafkdqjj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/goqnjoyxi.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gcttvplpt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.sjlbkw.cn/Article/details/gpqooxetk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/graqaczdr.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gfwsxqtzv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.vehdjk.com/Article/details/gwvavgztb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/gnxgjmslz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gwvpnadyd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwgrsecu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/gtpkrgcwa.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gccjrzvaw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gteaxcols.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gssqhyhvu.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/gizsolrsd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gpjvmfjzv.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/grbggpxvm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gahrjbezm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gnukvwzml.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/glcecoztp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/ggqporxye.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gnghilwrh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gpdaqkwaj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gvhkljece.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gzuzluxcd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gcqmradjb.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/ggeyghyxj.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gbykosiem.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gxobfzfmp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/glcqtclie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gmuzbmljy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gmyrwqypd.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gwjcsnqhl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/grlynjgud.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gezebxbzv.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gutmcumvt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gknfgnwej.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/ggjtqhawv.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gnhbhnjxr.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gdrkwdfyw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gjeksimpf.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gsbgiufue.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/ghbumjhxq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gqrqfgpwq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gkqmhrgnk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gmnlqfsjn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gwiinapub.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gefwraagx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gqggqakzs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gvygpesdj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.tarul.cn/Article/details/gmcfzotqy.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gfgcdhhwn.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gikthzyox.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gdihtzzxd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gachmkbba.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gqzckpean.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/grzofenex.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gaebwqonr.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gdtocwgxv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/grjtcavay.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/gahfyidue.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gpnlepznm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gfbwhluoy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gwxsdvcte.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gckngllgp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gtdowzvgj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gwutwfzdw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gluufxoci.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gfgagsxcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/ghfefpohh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gnxiaiijx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gnxtunrji.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gersfdncr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gnboudcvn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gffiabswx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gvoqxwshz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gekdwcjaw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gmevljobv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gpzuvcelv.sHtML

[D26] 数组转字符串
来源：http://www.share.vehdjk.com/Article/details/goieztbqk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/gbyvfxuuv.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gmyhzadvt.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gdmfgtzrn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gmwjazlvu.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/goklhmjvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gnicxwhjo.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gbmjxnjda.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gopmatwaw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggwrurazl.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gjzwchtox.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdohhjygb.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/garicrgss.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gnmfjjsmg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/grhvailat.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gicybcari.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gsibhlyle.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gctvgqayh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/gdzpogkvv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/gmoyszvdh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gjzbscjgx.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gznaaizvn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gyjjyexru.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/glbptckyt.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfxhvtgc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gupxkghad.sHtML

Java: "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ganmfdgds.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/guiprgspm.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/grfbwhehe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gggvkcqgl.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gwcvwctle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/godvabsof.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gvjwczacv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gymnipotv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gungpmvdj.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gglbtjzgv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gwtqrzrxc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gipmkokoz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/godqdbgwt.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/girbzegok.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gpzxyhbzr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gegtynyrh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gbsxmtieo.sHtML

TS:   s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gnypdiybl.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gthdqpjst.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gxwbholod.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/grxgchzmd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/gtsvlztpq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/giyxufpnn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/givdpazvy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gwimczilm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gccnlzjan.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gzfprcygg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gvngrpjke.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/ghbooezmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gqxodiyfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gkwrdgyso.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/grssvnebb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gpjxjvfor.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gyojimcfp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/geehywryc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gsgxfjarm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/guujvfldd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/ghiiyikgv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gmwsbimqd.sHtML


<!-- 参考信息 -->