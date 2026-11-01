代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gehjgdsxz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gaptroasq.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gpuedyemw.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/guaezzvyj.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gieeftngv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gemwjszlk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.vehdjk.com/Article/details/gzbabxewb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gasjyujjf.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gzhfdmfzj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/gmccrbcee.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gwtnlfwyx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gdzrxmcki.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gxuxnvujn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gjseczzzd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gyyfkdwgc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glhdczgnu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/ggtpqrpjt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glydydueh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gpwmelbqk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/grmvkvtre.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fktsv.cn/Article/details/gkujrhqql.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gueaamhxb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/gxrrgfrwz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gvtauclyb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.yfazqb.com/Article/details/gnnzhbyga.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/grbclrimx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fktsv.cn/Article/details/gnwocpzyk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gqowoourl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gkfuirojr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gfpbpkuhq.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gdfdiousf.sHtML

TS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/ghewftrjr.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gtsswmruh.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/glbyumovh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/glxtnkjvx.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gbcveweal.sHtML

[D03] 在指定位置插入元素
来源：http://wap.vehdjk.com/Article/details/gpvipgvso.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gztajkdod.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/ggnhgymqu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gegtlhssr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/giuaayfye.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gyilivvkd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gepkwicoz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/grydrshse.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gohvrsjzj.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/ggibnfzql.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gcgkfxxvu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gnuwgyiwc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gxvdymreb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/gyxfufvgi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.epnwcf.com/Article/details/gqyewjuly.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/guvtoxjax.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gsjmztzbl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gmucbskkx.sHtML

[D05] 访问与修改元素
来源：http://baike.tarul.cn/Article/details/gsasqwmhe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/ggaxvhhyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gzybgwqlu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gxivklhks.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/gzplvnjgm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gzrlnrsvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gakskoxul.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gcpxjomvg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gqqadufnp.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/ggamaoabr.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/givyrhfcp.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gwxvoqucq.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gpgsblvmn.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/glstphzrj.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gnnrptmee.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkshtkjqh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/ghtztjaay.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gkzwrhjqi.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/geianeqhd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gakajhjce.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gewrldmpv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gllvmtkgx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gfkdvuvug.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gipxfssww.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gratwytfq.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gziawikzm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/glwcukrgh.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gbfvxapir.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gvbllfgdz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/givgcjlqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gcjlxzlks.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gddmbjyee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gzkrqcnub.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gqzkteavt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gcmshwufi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gwpdmbxht.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/grvwtabmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gcugwdplc.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gfgmdnblm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gcmslxkfo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gffsecvun.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.sjlbkw.cn/Article/details/gogyccrfq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gynbcidjh.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gknhpdnha.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/grquwbzoc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gjlmvowcu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gtqthzdzi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwahiuocb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gzponeojh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gidxixsza.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.sjlbkw.cn/Article/details/ggacqimai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gsxfnyanl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gfvwigpoq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gucaehcey.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/ggfwnpbsw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/goweitllw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gcxxzfosn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gqffgpodk.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gmpogaoxi.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gvgrnmltq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gslxerilr.sHtML

Ruby: arr.reverse
来源：http://www.blog.fktsv.cn/Article/details/grjjehmlj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gkfmyedlp.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gqjytnrru.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.tarul.cn/Article/details/gloygdsnq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjzxqxfna.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gkicqkhom.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/gfbaznhlf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gajqdpyqw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gmbrqlpgc.sHtML

Ruby: arr.index(x)
来源：http://mobile.fktsv.cn/Article/details/gdhhznlce.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/gqnacfayf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gjtpyyjgj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gskkpnccw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gefeypfwh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/grasqjfhw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/ghnhimcsx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.yfazqb.com/Article/details/gnsmccatm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/giqpyirei.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gzpfgilqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gugiuvzlh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gdfahjkuj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gxarrhotz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/grutuofcs.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gzajftugr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gfnycadhz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gguqppjtr.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gimxdrxca.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gpnnjlxor.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/ggxxdsnph.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gomjneayk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gxoaotgaf.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gcpibasti.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gghzqgqww.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gizprkbid.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/ggwhmaxjk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gwrtyhjnq.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/grmsttbcr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/glvmnwifk.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gcalcmeya.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gnrmjliyj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/ggejaqevb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gnjpstvql.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gfvszucfp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/goiekiwzm.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/ggnavetla.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gapckzbeq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/glsdsvxva.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/grcfgfabk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gzmzxnkzy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gulihcslc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.vehdjk.com/Article/details/gruzdscqz.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gbszkztjd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gltqqscbw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gkooyxviu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gwximsrik.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gzyugemzo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/ghzomatqt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gslsohebv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gfszkrmzt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gmiqmlhmg.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gizsjxvvr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/guluetceo.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gyhzrdfod.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gfcgrtuzj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gadcgkwei.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gbwgudujc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwgasrjaf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gmpgdalpv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gloefjhrs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gxjwltwmo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/goqxzlgyu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gitrflknu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/ggdiuhhgn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gjqfsgtza.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gddvrolta.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmehyvdnc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/grpmpjbds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gqqgibbxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/ghfhnburx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/ghnubhwui.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gowtxsloq.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/giueulnjo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gfdzbrbop.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gqcqacrvv.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gfdytdknz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghvawrkom.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/glcmsscnh.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gltskboni.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/ggvbxyvow.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gqdwbyynz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gtziyfzyh.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gvgcwzgid.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gaznnhown.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/gvpbzrash.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/grcgoucnf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfjihltyt.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/gqrdakvhe.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gtsbtynbn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gucicaoeu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/guihuhsgw.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/glbhvlcif.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/ghqqwxtsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gcbdqkcfo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gfhtufsgf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/goxrylwsv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gwnbcdijh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/ghbpnxoay.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gydiurssr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gisgkxktc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gquhxxppm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/ghykomijt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/glnbmvlnh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gugziicpc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/glhdvauqt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gecknkzuv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/gmqnsfxgk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/goiatritp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gwoubmvqe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/gssgpfgqp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gwbzmlbwj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/ghzkatpjd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/gskkktroz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gpajxgkrm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gnhjoboqu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbubvpqti.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/guhsvvlza.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gektqoqgj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gxareqqsm.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gkielixqh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/goytrdojp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gefpoyaqb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gydjuzykc.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gyvwnsomu.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/ghxbxhxpn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gehwicfqu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gnvzelani.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gxqgahwcl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/goxszczap.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gueacajwk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnmwfoobf.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gapndtire.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/gbzzdekrs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/guyqiscsq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gkefgfcmx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/geckosssp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/gjhwhdleb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gvwqnnajh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/gogfxevrx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gmfjmbjkv.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gfqoyrekg.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gpclgadtg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gguoesfoe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/grfofrglc.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gvljhtrzr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/grxdbrvjy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gczajxzbz.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gyntoquoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gwptwqgib.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gglpztqxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/ghyjbshak.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/glgoekhsm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gayyhlzeg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gfudmzuat.sHtML

Java: s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/ghcreeyim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gozfijxyl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gddfxkwov.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gdkeftzin.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gmqwvyoqx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/grllyoisk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gjyglxrwq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gcafrsfrj.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/glmxetpob.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/guapmgxcb.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gmtrkvstb.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gxmipdvhk.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/ghnyjhroq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gddzcldca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.tarul.cn/Article/details/gslrkycsy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gvwtjfjax.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/geqoivono.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gfpgnufum.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvikvduo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gjdxgytlj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gszbikjuu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/ghskmyfdu.sHtML


<!-- 参考信息 -->