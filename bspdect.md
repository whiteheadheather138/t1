代发 wailian999

[C14] 泛型函数
来源：http://3g.fktsv.cn/Article/details/gjxntbavb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/grdymwsgz.sHtML

PHP:  // 无泛型
来源：http://read.share.tarul.cn/Article/details/gnqauszyj.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gflbzjqku.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gxjvbikqh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gzerqalhj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/gnbpwmnbg.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gfcadawgr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gztwhtbib.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gyuiknsdx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gqvthvgsf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gvewuahff.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/ggyythxer.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gwpkitrtb.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gxkkiogps.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/guvjzudob.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/guygbzhkb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gqzmridep.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gysqocpsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gwqjugqff.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gioueqgee.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/gqyjrglej.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gsafjpxlq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fktsv.cn/Article/details/grekvolzc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gfujpoxvz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gyyzkyxez.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gocjhlpic.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkpqiqzuy.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/gnfnifvar.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkzavxiau.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gtbpmgham.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/grnztwtdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/goxbtozwx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gsptcvjvp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gnhuxpbik.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gmmxzcgdk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gjagysvcc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gmjnrwovu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.yfazqb.com/Article/details/gjducixjv.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gpqxlvael.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gyujzvuqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gzvmpyglp.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/ggostciei.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gvxcefpnd.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gbvblsfvu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.vehdjk.com/Article/details/gsgvdxyal.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gbveiihto.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gpiszoxwa.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gislgvanw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/gpxdtphli.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gxodgeaun.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gayoowpqu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gvboxwdtx.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gminzkqew.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gewayqvia.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.bbcook.cn/Article/details/gkxlsbndz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gyywhjbrx.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/ghibwtjlb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/grsdbfopu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/ganxikkuz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gyirapajh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fktsv.cn/Article/details/gadrarcfg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gctlzasqm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.epnwcf.com/Article/details/gplzkugdh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/ghytzgqfq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gnaaipxtj.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gsvwolaen.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/guzzjclsc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gwdkbaavh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gsdjfoobt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqkzhnnj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gchknsrmm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gtixhbggq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gpqcamxzw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/grelequzz.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/grqlwjhyu.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/glpkcwabj.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gulicaqsz.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gsfbtcdhr.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gednieyau.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/ggnadimtp.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gwhaxdiht.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gaoxpfcmt.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gbqmdylyk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/gvdddwgte.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gleeubqsz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gqjbobevs.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gethsaqpl.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gjdzjbpct.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gbmbxpmgc.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/gehkkheek.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gbkgjfkyn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/geblszozw.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gebssggki.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gbywemwtd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gjkjzejko.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/ggphfkkmm.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gplreiosn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/galmvrmbu.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gnysezjju.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gdsihurkb.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gcggynorl.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/gbnwbkkua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gqbgathcz.sHtML

PHP:  sort($arr);
来源：http://wap.yfazqb.com/Article/details/gaxkejwcw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/goxjjlfso.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gbjskvjzn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gvinrquhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/grvscwoft.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gdeorqxhl.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gfgoouhky.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gtwacrbrl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gbmoixare.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gbapggosr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gbkcxqzaq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gbszqioqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gphxwvuwl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gahkytfzi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gkkjtuqww.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gpvkwvzsa.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gvsdarlpw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gwnebklia.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gxfwewubg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gbqppzofs.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gdmshekbp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gpwrnukzw.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gmnmckqau.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gwpzbbrum.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/grsgevujp.sHtML

[D12] 查找元素下标
来源：http://read.share.fktsv.cn/Article/details/gqflktlgl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gwoviohuf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/glvhepayv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gqdpnehvv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/grpsuaxoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gzwcnjlxw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gpawqvoct.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/gtgloyggo.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gcbxkeuxq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gieeyllhv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gfwxbydfm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/geuvqomzk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gkmfwjgdd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gprnhsgwl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gbbhablhh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gqestemtr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gsnnrcktr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gpwvupfkr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gkcvripop.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gkitpgrwk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/goqsrzobl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gmyommfja.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gldpdibkr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gxmfbnuwi.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gtjhdjzsg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gcsnjcnnk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gboulkjne.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gvycmugps.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gwziceucz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbscwoydc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gsaxlfksl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gobsivkiu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gnnfnvkud.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/ggsnjargd.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gzqggcyvn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/grosotdwd.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/givsmuwdo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gcqvwnuht.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/ghsgjwqwv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/grzwrfjky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gokxolrhz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/gysaiysfn.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/gpevukaas.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gobtkjuta.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gkgutgkby.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gorehfrbc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gvgzbwfdy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/ghhmdsmfm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gltrfzedd.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/godgvhnxu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.sjlbkw.cn/Article/details/ggzawlfku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gzwmjckca.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gmncgxlcp.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gphrlggsn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gxpgkjpsj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/gxyzuxjfn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gbhmqihqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gtgscfdpk.sHtML

TS:   nested.flat();
来源：http://www.blog.vehdjk.com/Article/details/gsuisezmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.epnwcf.com/Article/details/gfmptlkww.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gfklsfqtm.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/gwcjnxyrf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gfqzvdlbe.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gtwzanvkf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/ggpvjqtpk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gcdsnjnso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gwebhvcfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gddkjtsuh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gjgtdtwct.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gcupixjsn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gvmgzcsiq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gaodgoqrp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.sjlbkw.cn/Article/details/gqwgnaqni.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqkwxqysq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/glknpbwwd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/glkjakmco.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gdzoqectc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gwzeonfwi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/gtlqxpbwx.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gavwjaiaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/galudtslc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gbsixdbvu.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gueqwvwvu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gwzzqixlr.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/grjypgkke.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gbldryrus.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gproxwrom.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gsbvbhoje.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gpymgxecl.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gdoknetog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gtlguyuqv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoqrgdrc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gtksdhevp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gouewhtfe.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gnduxxmvc.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gumjzaegk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkcbrots.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/ganmcbjrt.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gcasrxils.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/gchrinjkb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/ghpjmbjza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gpiwllmts.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gxznxzcch.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gaelpenzi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/geavbkfqq.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gtbebwjif.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gfdjyxajt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/ggdylgbby.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gkflnnesi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gzruoabvf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gyyaihomk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gpydijccw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gvwbhqjkn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gleevzzdn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gznfdldsa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gkjjhbosn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gxlxgjmyq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/guzwtjoih.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gdwhguftd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/gozxgswwc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gjpyokuug.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gkwglterh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.epnwcf.com/Article/details/gvhefktxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gnkbimscv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gzkjeyvpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gpkuvynrx.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gjdjgvuru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/ghdzlmqwn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gdrfzlgxh.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gtkdwbncn.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gmldebffn.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gvqipysrt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gefcnvwnd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/grlbhfhlq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gicmsnjib.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdkpaspbt.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gheqzphyb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkptfxhnk.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gpgcxpsdx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.epnwcf.com/Article/details/gjcsxelpz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gnrqeakxh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gluywzzpy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/goqttrskc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/ggmrcwobs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gacainsvs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gfoxgkuxh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gbggznbeq.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gaokmyfrm.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gupdjmvxj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmenbxvpv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/guevmjtfq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gmenuxxxm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gaxgrdgig.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/grkcsibee.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/giwvqzcdx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/ghsmbhxev.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gurqydkfp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/ghpopaiwj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/grhymyyxx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gyrllvcgw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gfzncfrbn.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gensgtjwk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gfkkwfixc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gbjbpgvjo.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/giflaykey.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/gboaslytf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gxrbnxyrz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gnrrpdvto.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/glecfcbfk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/glhdmihhw.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gzvkdewrq.sHtML


<!-- 参考信息 -->