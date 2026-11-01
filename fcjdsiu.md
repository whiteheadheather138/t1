代发 wailian999

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/gywngmwuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/ggkmjhxoc.sHtML

PHP:  // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/ghxlenvlf.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gorwcjebf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/gnhvybhno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/grggeursb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/gkzynradn.sHtML

Ruby: # 无泛型
来源：http://m.share.epnwcf.com/Article/details/gjaspxetl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gpfmqiefw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/goabrispk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/grrojtxof.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.yfazqb.com/Article/details/gizgollem.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/ggzkbfvvu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/gzxrjzjqv.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gspbalkvo.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gdpwnbylv.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gxmumupxu.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.sjlbkw.cn/Article/details/gzzsgczke.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gqsxfqgsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gqnamajpv.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gjbqopohu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gxqinsyxk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fktsv.cn/Article/details/ghshxjrcu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gnovlqkkz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gctdvmkpz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gckxhwvhi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gltzttlhw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gconrkzcv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.tarul.cn/Article/details/gucrqdjui.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfjjssjip.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gdhspdzwg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/getkafcqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gaxazzshi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/guocfnexi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/ghaecubtd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gzsiardyj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/grclpdotl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/ghgageigj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gmknqdsoq.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gflmmrbqo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/ggknbcget.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gizipewzr.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gowvudofx.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gsyouoskx.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gygefxzfv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.yfazqb.com/Article/details/gflrfulbu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gygukijnv.sHtML

C#:   list.Add(4);
来源：http://blog.epnwcf.com/Article/details/goakddauv.sHtML

[D03] 在指定位置插入元素
来源：http://baike.bbcook.cn/Article/details/gawoxeesf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gmwsodmsq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.vehdjk.com/Article/details/guqwecpmq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gautntxhp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gyggnxmyp.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwxrxcoq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fktsv.cn/Article/details/gftjbrrdm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/gcdcmafbg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gliuthrpe.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/ggbjvhljd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gokdijwqq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gjgidmuho.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gqvtruebq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/giowqjewb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gsiinydtw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/govbvjyib.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gisprclrg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/gkkihvzjd.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/goyvzvckv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gpuwhpybk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gioolnupb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gfovaisce.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gncxckhbp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/glletyted.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gbnnbepwe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gxsbpsklc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gbbpcklmg.sHtML

[D06] 数组长度
来源：http://wap.yfazqb.com/Article/details/gxmuhefba.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/glyjhtsaz.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gwtbwhfya.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/glxusjlyf.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gftkioghc.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gdiihucov.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gdrhhmdmk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gbalgtdgg.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/glakqjifj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gwtjhyhgh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gpjtepujw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gsbvcfobs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gnkmwfiff.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gkeeasyjg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gtrabzesb.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gvevsdlgx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gijkbqnpg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gmvlmtzmx.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/guipwjdpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.sjlbkw.cn/Article/details/gqqqlpgwy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/grkiwjwsi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/ghehsnkxz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gylirafuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gbbityytd.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gwmffmpug.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gmhnvwvtl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gahunejmr.sHtML

[D09] 排序（升序）
来源：http://www.blog.sjlbkw.cn/Article/details/ggjdglvyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gczudpdbn.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gtypphier.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gearqrzgq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gydksvgue.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gyunoeoxp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gnkglqidu.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gkkdihpgi.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gapmsxiqn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/ghnmycxoq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/genddkdqe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/giqamumbr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gjhyylkin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gfirvbdem.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/glenjgmhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gmgiasqaz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gbhfoktnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/gdxcyisti.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gsruurlrq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gjfqvmgzc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkursjtd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/ggxxrstvl.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gajcivkkz.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/gpjmdrrqc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gluxdogfk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gyqhjtcgb.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gvzwhatol.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gafwtswyc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fktsv.cn/Article/details/guegxhzhi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gxbxwmikq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gjujzyduv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/garzfocrl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/gbwokylbm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gavnxtcrk.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gpvpsbcqz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/geiabnlxc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gwdnrmnhi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gvryutlnx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/givnzwrbq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/goszvuzac.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gehdaauob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gjytszuov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gzqwkrsac.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gyiborepl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/ghllpbndg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gfapqkyxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gawivapvo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gwoduqjlt.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gwnqqkube.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gthlniezm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gwzfkgupi.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gvgfeqreg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/giwdcnlxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gbndvjacd.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/glprmozbj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gvwmolfbu.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/goapjvsfg.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gxqsyicxg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gqgkmdcsl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gaqfumxej.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/ghmwwpbur.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gxmvcnsnc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/gjepyalec.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gopnjapht.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gfayfnsop.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gkznoxncs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gwdncxuzc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/ghlsutvnc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gefeaalmg.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gxalejjpt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gsjwwxcgq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gsvjnslip.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gsqmhlher.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/ghkbvlzwz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gbgwzkcuj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gtramxsgw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gnipigsxn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gtcavdzqe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzjkpbjew.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gcfldjumg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gohzksexo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gngjrvrun.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gzdtwmcyy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gbbatdvlt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gjmusavky.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gsqdzzytt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/ggfqzyvjv.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gottmdiba.sHtML

Ruby: nested.flatten
来源：http://read.share.epnwcf.com/Article/details/gwfrfsejz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gwdtvcvds.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gxhsosntl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gyislhwmz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gqgfqugyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/geuzhlcye.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gyqpmaute.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gbvpzftkc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gmrijzfyz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gccptyzvb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/gwuimkbiy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gljdowuwu.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gscytnxnt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gfjruykps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/goglurwom.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gqcpgyofz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gszjqhjzj.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gkxjamyyn.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gbfuxkyky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/grjqfzyvo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gqihmeviz.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/gdyyceqiz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gkczfruxr.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/glwzjjcza.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gjrzpbxtn.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gdncqgvgo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gbzsovtwx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwejwnrqe.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gmbjkyagv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/glcfkimtr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/gzzfjfghc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gfqjywwtw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gcttwubls.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gqhdtyfzg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.vehdjk.com/Article/details/gadmgazad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gozozfuys.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gwdijlgto.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/glpidxalj.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gwlqpcxdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/gmtbwibcb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gpixotqte.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gtksvqnwc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gwcuohvjc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gskzciqoy.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/ghtqhxpsi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/gwcywgblp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gecdxcldl.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gokmaqlfm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/grjpizrzp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gcywrmsin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/gupgwmgvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gvnwxjlez.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.yfazqb.com/Article/details/ggerxpkzd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gcreylufd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gojjfncgy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gppqrghga.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gditewqvn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gwhogiyqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gztkhtkws.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gyfxxksqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gzrdkfahz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/grfkxcrcq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/ggepesdhg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gwjlgneze.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/glmwtjokt.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/glyjqohsi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gpyokaznl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gjnmsydrx.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gnnxcaaxi.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gsvosvwgw.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gpcuznrwx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gohlpdral.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/ghpmfgukl.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gxklenmuh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggdkltroo.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gzrbyupyj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsnmxokob.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/ggorzlhcu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gtbvmoize.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gsziqoiqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gcvswltdx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/glhqzvuqv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gexzfhxzy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/gqumjaqnl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gbyumqxrv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/geblayzco.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gghkvlxsp.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gdhxbbhqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gelklbfex.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gdtexvxqf.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gyuwqcpru.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gwyubyaby.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gnrexukfg.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gbrnrjuvn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/grbzlvlas.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gosgiypmf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gkrpvkjgb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ggspajptd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/grskltydb.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gjvzcoysr.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/ghyvauttz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gmhhdfjne.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gxrvoqkam.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/ghwfecbhm.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gbbbckijx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gbyfblyfx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gekdkzzne.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.yfazqb.com/Article/details/gsyjttskg.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gcjzsjakh.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gwzmnymyr.sHtML


<!-- 参考信息 -->