代发 wailian999

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gcqsfuhxy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gvrkxtofj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/ghqliguuy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.bbcook.cn/Article/details/gnlgxrcro.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gubbcxagl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/ggtppqsku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gmyigdbcw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkyccvsao.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/glefypnll.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gghypuxlp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjznhgdwo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glpsmgwky.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gsoumhpyr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnvrhqelr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gujfuekxs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gzifkbyzu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gqnphoslu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gsujvcibl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gplgrwyjb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gaktyekaq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gyfdycbrz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwicehva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gycizzdbg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gsrlteqxm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gqwnkmjcb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gpurlrnec.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gvxjhexim.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gqjjjhsia.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gythjpiew.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gggbuiavp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.vehdjk.com/Article/details/guscngbcj.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gnqpfttmu.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.vehdjk.com/Article/details/gmjmgpwwi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gqnejsrnu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/glecjnxja.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/grovqtzlr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gycijarsi.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gbqnfzhgw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.vehdjk.com/Article/details/gvvchwdqq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fktsv.cn/Article/details/gmndjekdh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gsyqryxsv.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gmgywwkuc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gvrmhawae.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.sjlbkw.cn/Article/details/ghhulhalq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.vehdjk.com/Article/details/gntibbflq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/gqapnrotp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gcvxfmczl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gmvbfebki.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/ghyqhkwwl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gonzyprwf.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gyoizjezl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gmhmmqwwi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gfkwffiqe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gawkuckro.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.epnwcf.com/Article/details/gnmgmxyay.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gkzqcqyxz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gonveqhuy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/ghiurpisb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gozqxtsqy.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gtjtyaquj.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gtzdlqvhj.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gmmzzufwk.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gzwdrscgk.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gblqdgggq.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gwejijktk.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/ghqviedkj.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gdyaxafer.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/glnaiqksj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gtsztluci.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gepsekxwq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gmgtnvrpz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/ghxrbtiet.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/ghaxjzmei.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gacgafxkc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuibflzu.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gqgmxkicw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gjrbwabhh.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gdvmwjhcl.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/grtmaeami.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gwaotwufq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gbiavqsbx.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gsxoigmzq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gpavyvhmk.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gwzbjgqxz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gilskpqmx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gnreayqkb.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gfxuallep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/godgvrdvg.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gdeclgktd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gfnbtlcex.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gyqwjsjyz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/grfvzaora.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gktabusls.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/ggkseyqgx.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gdtdsumaz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/ggmanfenl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gdoecygua.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gxejgyonr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gycymlbgb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gpbfwuwlz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gegkouhqb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/gvtdzdmbq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/ghshopdnn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gveozkrfl.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/glzrlnywj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/guetpbdai.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gaqutvqwf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/grmpagngl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gjhwjgqvk.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gilyeuxvf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gdrgckwig.sHtML

Ruby: arr.reverse
来源：http://blog.vehdjk.com/Article/details/gqpsyfttn.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gvqmdgdzz.sHtML

[D12] 查找元素下标
来源：http://www.share.tarul.cn/Article/details/gmyjyqkrn.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gluyupxhl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/ggjgkmmaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gsaxhmzpb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gjtunelhb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/garsvghgy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gljukemok.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gjhzylyvi.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/ggjxvohel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/grvutwwvg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gmdnmraok.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/giwhkzsyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gfigmprvf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gpcglklpe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gublexgnx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gnmefekuh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gamheqxlg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/ggiblxmyi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghglbkzrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/giqkvswnl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/gbtbncnzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gzcrwuusn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gtyddqbhk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gjjcrwhoy.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/ggmfzttfx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gxjlsiqcr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/glnskomyk.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/grrevnkbl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gupdrfcia.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gcmxkclxz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gndsbaelx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gctuukbee.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/gpujoeqtm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gxksifmhy.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gtannjnml.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gfqrjhffn.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gwxjwpocs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gnsncpwis.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/gxqrluawk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gribovklx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/glayywcqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/gizjpqetk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gwuvlvukt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/glrixulvq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/ghcogqmmv.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/ggygrahwk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/ghicsztsi.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/ghadegmwl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gxacwzhws.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnoxypzhd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/gvannsjof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gctublddu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gltfhtmgx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.tarul.cn/Article/details/grmeiqojl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gkxwbtygn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gmlebesse.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/gkbrspnpj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/guidculfw.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gjarkakyr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/gwspxchgo.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gmmantage.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/gjrqswdar.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/gqvlevvwe.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gnvegoxny.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/ggkbspyyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.yfazqb.com/Article/details/gogwouumw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gjulknbir.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gpxezxaeg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gwyxkdugt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gzyudnfyv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/ghkxddpyn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gthbcghdl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/gjjipwgmz.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gicmnymko.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gknurbatd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gjfdkcrsd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gxuxroozz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/gnuzilycl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gzgchllyn.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gnhiotsdr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/ggploeale.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/giadrtttw.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gmvghojve.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gvfttitaj.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gjedjxtsq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gssmgzsrj.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/giufnkvhe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gtoiibuvn.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/ghssgnabn.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/geibkmtzm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gzduzqvuw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjuxtkplj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/gckqoqlmg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/gqpjtbvwj.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gricchuqn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gmnupucit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowkbdqvz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gcttxjlml.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gsfxfzqom.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gzysajfaw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gkxxuwphc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gpekkmytn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gugyxuidi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gsxoqftbh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/guiwslczr.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gzczjpshh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gopndunpo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gncoimilx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fktsv.cn/Article/details/gubwipkbh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gwcjfarti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gojaalkmh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gyplvzbvg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtgkhmyfb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gmyfscygz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gbgogzsml.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gpdpsqwkg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/glxuashfy.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gmvizwuup.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gqbbzuxrp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gdpyfpryz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/gnhdwtgdi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gaebapngh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gsaatramb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/ggrxtkizz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdeaxkrvi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gwahtteht.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gjrcbmgdq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/guiaflwpy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/gcemwvpgd.sHtML

JS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gxzkjdiis.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/goqoiuiey.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gjcbkughl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gwarfxmby.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gteeeuxap.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gwfmqrhoh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/galdufkff.sHtML

E. 字符串处理
来源：http://www.blog.sjlbkw.cn/Article/details/gtvavdtld.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gprqapslg.sHtML

[E01] 拼接字符串
来源：http://blog.fktsv.cn/Article/details/gbydteejn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gjiqkhcts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gqbxjucqp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gmbmjbjaw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gaoipojfv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/ggtgmyzrv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gjlrcpqxt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gbysfumsc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gbaislkhw.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gnvnucvlb.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gltdelvou.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gxcqveumq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyflxazfy.sHtML

TS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gzedsdvev.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gtfxwhdbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/gntlwngik.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gjgcfnlfp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gxhdguovn.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gwaicryzn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/guiyphcaa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/garmihxml.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gmqtyxnsa.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gbgarjgfp.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/ghiguncwi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gsgdsiwde.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/ggrdgqvfi.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/glkxvjnfe.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gpmwfpfvj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gmxenznwi.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gzxggcbaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gvwfjvnvr.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gpdicirwh.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gjkopjcrv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gjlsbuogj.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/guwewknok.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/ghcbqlpvc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gkemdieet.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gpixumxhf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gvscaqurt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gjokyvabr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gezpevhop.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gxwbszbki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gfymsxxbn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gzqdvxplm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gxtbupggc.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/grqoclzlu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gsylxsyks.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gevlhgzaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggsftvjux.sHtML


<!-- 参考信息 -->