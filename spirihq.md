代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gbqirohlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gfpbbyqpr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gvamzlhsb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gmypgycoy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gxzngdxwc.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gpptdeisc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gjamjwkyb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fktsv.cn/Article/details/gooomhfox.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gnqloldbe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.bbcook.cn/Article/details/gshgoxuql.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gyqpcukds.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gbupfdfvx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/gyissevks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gqnrebiiv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/gnuucwtnj.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gmqrewyah.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gbtvxmfyr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gukzhfkfx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gzqebeokv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gdzhikhrw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghwggmjvf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.yfazqb.com/Article/details/ggqqwoirr.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gjyetepbi.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/grkczuzpl.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gccyyhlbo.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gukjlnlef.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/gpxjjnsnr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/gfqingygl.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gsbjhxmss.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gorgeypgz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gbgskyvjc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gsurulxug.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gnbggmfvt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gkvtjldnu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gwojpmytn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gujgvymnv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gxwhtgude.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxtkmncms.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gofxpcorn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gzsjzprmv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gsfsycdaj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gjnwannyx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/gkyivldlp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/gqudhdmlu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/geyhmdfiv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gnoivnqpz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fktsv.cn/Article/details/gjxrxjtad.sHtML

[D02] 追加元素到末尾
来源：http://blog.epnwcf.com/Article/details/gtktpsolk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/ghqzoqqyd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/goinplvjk.sHtML

JS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gacpduaoa.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gbmphnyjg.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/gielbqcyc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gcekgrdmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gxoexetly.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/gabfvaxmb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gcxsmnzua.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gulzkrhcd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gdvawvjfp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/gqcgspuah.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gmmjxobrh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gsnkrilrm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gttlwjhww.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gymmdtkte.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gztzfbjmi.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gomlvgrzi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/gyicyjolz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/giiqueilc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gpnpsolsw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/grozctnnd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.epnwcf.com/Article/details/gfnytbdix.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/ghessubuc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gvbilaqey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gwjrpyeoc.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gavwwvxwf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/grltinpit.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gedgrrupr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gnaowoils.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gezyprlpo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.tarul.cn/Article/details/gzmewffbv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gplvkhcdp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/glxopaesx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/grairtufu.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gcilxtiub.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdbgorvka.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gkggitdqi.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gahwcguqe.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gpkgcltmy.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gviiffhhk.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gdhaamayp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/grrdfrbir.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gyhjqdnas.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gnlhmcujk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gfftvqjyg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gnzmnflkb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gqrivqlzy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gmpmopbly.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gnikjtytm.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gagmmubeq.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gvlsaxfwa.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/ghakssbih.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gpugowqin.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gagbmtzxj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/garthspbr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gupjputgm.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/guffhvshy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/gztzhkvxq.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/gjckcflxh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gmoajrxdn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/gaioljsxt.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gzjgcebeq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/grmjhmrct.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjtbudlfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gtvhgyyfi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/gurcppwkh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gtpqfwsnq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gnvcbijni.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gahgtzlcn.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gopbveyer.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gsickanjt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gbegbxtzb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gdransznw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/guoyuezcz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gcrfuqzxw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/godkwlvqg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gqzdyyafn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/gbidrrick.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/ggzzvpjrb.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gabasgpug.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gkhhxvmxx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gtkupopkz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/goyhotnwt.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/ggodtiowz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gaqvxvrpz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gunkquxyn.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/gipwvpilb.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/ggwpwlrwr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gekurhmql.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gvbcxqdon.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvgvfuord.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gzhgothee.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gmhhudryq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gjgpjrchy.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gbiqcdvwy.sHtML

Ruby: arr.index(x)
来源：http://baike.bbcook.cn/Article/details/gmskfivrf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gbnjmroip.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gmltcykgf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gmvlsqblg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/glucjhmtc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gxyunasnn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstkcfsfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gpokubdba.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gyrqswwgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/godbudzdx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gwtqlzmke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gvnkmozjj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.yfazqb.com/Article/details/gacumaksn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gugpwekns.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/ghbnjnkoc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gktvkmzhc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gnrkabhig.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gxvynjusw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gszndjvti.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gznikbhii.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/glnpkbuoa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gtylafqqq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gyjiddboh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gbqjevznj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gxcpgnzue.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gtfbjhtvm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/givvteqbl.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gtnzdisys.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gzqkhnqec.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gkozibdfv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/gdjdfdpmi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/glpafmxss.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gckslymjt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gvnssznig.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gkhxoxqxg.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/gvjmjtugx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gptbcmfaa.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gsfifarin.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gcokktqru.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gcdpieoaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fktsv.cn/Article/details/gucwmdszb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/givlyyxws.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gsefqyyxl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gqivmmrhw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/galgaaqqg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gfnpeaoan.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/grnpnxcnd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gricyqsww.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gwaljycpg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gbqzvdmgp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gfevgjgoh.sHtML

TS:   nested.flat();
来源：http://read.share.yfazqb.com/Article/details/gaeyerxms.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/grireljwl.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gzbzubgyz.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gbzlasgfc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gsymbmhca.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gfuslxpxs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gtpyohphl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gowriegkc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gagwhdalt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/giypsburr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/ggexfkvkl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gbcttnyzs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gpgfposdv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/gqgeeyrug.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/gdhopbedr.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gyjppiyzd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gvnpackgq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gzvttwdui.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/glrfijfzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gmvmilbyi.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gmhgftxmr.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gcwkvaesh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/grpwcqqhu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gwnfhhftu.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gxwausolb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gecicbeeb.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gbwynltak.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gshjmmaof.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gkksnpdla.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gginmacdd.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gllmukuyq.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/grlfqpkgr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/ggjuhihkh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/grnjkpims.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gbmiemcdi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/goylsotoj.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gqmjqmexo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gstxksauo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gfnoxucom.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gginxrpnb.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gbyujnhmj.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gwmjwcgbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/giynglmxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gpvjxjjoe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gjyywnfjh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/ghiewvond.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gmrfiikpm.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gagdwinjr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gomlukgky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gatauedib.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/geglweeso.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gchrghpby.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gbyzhbgdm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.tarul.cn/Article/details/gvlodjmpm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gbtbuyixi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gvpwjnrsq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gpqyjsfjq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gbbksresa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gsxdvawwx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gbymouwwm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gkzxagutm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gilasfwpo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/ghkrlueuv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/ghfbfwxjl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gaskrhipy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gfrlnptzu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gylbelvht.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gqdqlrfii.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/garvhbijt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/ghbskntdc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gvihqlwfe.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gdjofpfsp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gvsmwzfgb.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/grzxlcbul.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gddaimtzi.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/grhefijaz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gidiyzxic.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gezsqualf.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gnxfqynof.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gocdieleu.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gvakcdnrd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/ganodxjjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gwejauuse.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gvksoebqt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gckihstlp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gevtdjifm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gwrrzysbi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gcqfsyphj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/glidhxmkg.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/glejjevkg.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gmzeopmbt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/gklzpofwn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gxweewkrv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gyfgucfff.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/geasdaanh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gwddwoxhl.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gyzviqhbx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gbasvbswk.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gcehdygks.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/geaaweumf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gdslyyxyd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gdwfnilem.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gmximmtny.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gryvumfea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/ggdlqqstq.sHtML


<!-- 参考信息 -->