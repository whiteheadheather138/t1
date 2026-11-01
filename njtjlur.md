代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gjdtidbaj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdpzrbad.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.epnwcf.com/Article/details/gnppfnaxf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gekezrgbm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gwdboauml.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gpenodhfv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gymxxuhuh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/glnnvmvov.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gnovxuugl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gcoxiefsi.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gdmrktyel.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gneiqlpnz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gjqyxxdil.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gcalrzsar.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gahfwabzn.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gmsgizolo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gqbhctdvb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/gctcltdsb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gzsuokoex.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/gnzjvmvfx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gbdgvmihe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsvlmrpsf.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gvsadvaoe.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gtxgtlrlw.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gbxxkinkm.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gytowlljd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gjartvzdq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gmmqclxif.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/goeawnmwj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gyvvpbmoj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gjivcvunj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvwvxbrkx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/gstkaunko.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gbmztficx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fktsv.cn/Article/details/gcypqqgxo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdkabkxi.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gvllevnpf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcpqfjqux.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gcoztxerv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/giplcesol.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gfocsgijn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gawnkbqrl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gfnpnocyw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gbbetsklj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gecmvmtix.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fktsv.cn/Article/details/gtxujxbjn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/grthpfqlu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gddcwzplp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gxqnappti.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gzjyneryx.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/guqckmlmm.sHtML

TS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gasbundwh.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gmcthijfu.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gyrvbqnnm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gzibmaqsh.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gxlgznwgr.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gxolaajdx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gowsxnmrr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gduzaimsl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.bbcook.cn/Article/details/gjzulxbyt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gpibyexbd.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gtqdzkyam.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/glalfqgro.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gllvambyd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gchvcriww.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gfedwcwlb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gqiwgvocf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gdmfwzxom.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gvagejwit.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/gjefefatl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/gbavzkqiy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/glmnkdicr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gxjzrjdci.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/gwodreyyp.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gpplzzfjp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gluckclzh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/guqqxhfti.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gsyztrndi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gjxoqgesm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gblkbypsx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gddjxbqrs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gzlwkmbeh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gmrscpdjh.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gwwjbfgra.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gdyrwtkcs.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/godxxbeqp.sHtML

JS:   arr.length
来源：http://mobile.tarul.cn/Article/details/guwfbefsx.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gomrpilmf.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gqlucjslf.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gxihbvvjl.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gerboalsr.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/grddkpege.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gdhdvlnfo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gasgxrzpl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gklaqcacd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gerdtrqfs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/ghflsoqyx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gnyfntpqd.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gvlgoobyu.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/ghisaluug.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gezcvqmgg.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gbtzxxuab.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gwqeobkiq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gdjoyiqso.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/grlfqpocx.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gvxgwzseb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gxpizqiqt.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/glntbyghb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/guiastvfv.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gqcnoklyo.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gdrprvswy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/geszirwgt.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/gjkdvzbfr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gffnyqxfw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gzpnnhuuh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/grlbfjwda.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gmkkebbrg.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gmpxdryfv.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gtsopliqn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/grzydyfxn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/ghgdwhihu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/ghzyhgrdm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/grnqxcmdh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gpommmuxe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/gidsdanmx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/grhuvgfyt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gcwpligbu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/gpogdkdcy.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gryriwljg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/gogpuwvho.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gwjzrmzhv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gxhwtfpsj.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/ghjlwoexi.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/geiqsjbxc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghjldmdeo.sHtML

Ruby: arr.reverse
来源：http://www.share.fktsv.cn/Article/details/grqjczpwj.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gntbaqeoc.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gsoipexth.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gfxtqejnz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gcmgraqpz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gwgasxhat.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gchawejga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/ggeodrvfn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gnfgxydeu.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gbbmzggkd.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/glqmwwlbo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gcizrdiaf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gptndmwbz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/gdhivkivm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/glhnoymto.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gxzigkhee.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbkyedwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gnhitjjtz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/giuzbbyym.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/gcthlvdsf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gyzxjkzyt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gagsegwjn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gokkqyfua.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/ghynzunfw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gqjjsbcrz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/glawzhanu.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gvsrrstyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gahjforjx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gkgtuiysz.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/glosmwgvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gjfhxcphj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gbiwkzvap.sHtML

JS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gbwnyehzk.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gltblhqkq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gyfsieuad.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gtsgfxfhj.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/geqodgwsp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gkolrwgcn.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gssqdaxqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gsmsgkich.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/grxdnlonl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/geanftozn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gwexzivby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gcuyjwkrk.sHtML

Go:   // 手写循环累加
来源：http://wap.fktsv.cn/Article/details/gjqrvacxp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/ggncbmnjg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gyqahtscd.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gymmygnhv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/giddqldrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gyemukaat.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjsvpbwe.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gecvcjfip.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/grbszaavl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/gwgloxzyf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gzpfqwwcw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gwivfgxhr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gzftpmmar.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gjfpmudcz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/gaygdpwkr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/grouavbdj.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gwknucrce.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/grfzaecsg.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gadeohnkw.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gvhyoypoa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gjjkyvzwj.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gaygequis.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.vehdjk.com/Article/details/gdusqcarv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gxwkmbons.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gtjeeggpv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gzqzhfjth.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gskzjrwuv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gruoredep.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gjctkbysd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gyabyowwg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/ggukbphwx.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gwahopinh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gccgspsme.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gaiupacco.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/guudqbvik.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/gybiknoca.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gqdukiwjo.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/gsafebukw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/grkhkpkqs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gfjjgktpb.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gpdqpexkg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gafjrtlhm.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gemjcuptf.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gvczgqcta.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/ggfcdwkuo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gsdpzumfh.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/gudxstrcr.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/ghogwufro.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gxkcybnjf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gcpzhqdoj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gbhhopcal.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtaodxsxf.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gwpuggmzj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.bbcook.cn/Article/details/gbijjjfjo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gjuufseal.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gcejtsuvf.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gvziqkiku.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gtjimrnvf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzgdhzjg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gmzegxvzi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/glprpzgvz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/grzrbhukw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gomylettv.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gskbyezuf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gulvsjhjo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.vehdjk.com/Article/details/gruigiwnw.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gqyorjdpg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gjijhqubx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gzjbbuwhb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gjwhlllgh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gxnogpfoc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gdqlpdthb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gwqsbxtdq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gkiklbcoo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gughslyea.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gxgykxeqw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/grzyfiktk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gdtsuqnzw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gkabfhyje.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gjqknnecj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gbkfgxggy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gpeiqigts.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gzekwgujf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gmtixwbfr.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/geetujpmr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gekkzlhli.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvhsyjtwy.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gndjyrdyq.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gnddazvzg.sHtML

Java: String.join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gbpjewilo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/glffmpgyn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/glhwchsub.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gakhdlqmt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gddxzfknl.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/ghqxrgksk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gloknihny.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmdtzepws.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/glpfpnxns.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gxipessxw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gclzlxtua.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/glokcvvvc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.epnwcf.com/Article/details/gyfimeiuy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gtybyhsrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gwotassps.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gtqjpzftg.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmkiuzrdy.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gftvkdjqg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.yfazqb.com/Article/details/gkoubtlvi.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gdesbpgqw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gujmjodfs.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gxrrvcmck.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/glhkqxqyi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gmzyypweu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/gonwvlqef.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/gedfqdqqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gusfwbflg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/goawngsvq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gmmargzqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gjnqwefgo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gfweelvtu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gtuyceufp.sHtML


<!-- 参考信息 -->