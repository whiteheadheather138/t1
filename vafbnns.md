代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gljqmywvi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gilutumyg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gerozcqmz.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gjrehnulp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gzteptpqp.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/grxbknvwv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/glmelvkwe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gezozlbrn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/glagrrdeo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gnzzzszuz.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gzjapvpkf.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gafrmubmj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gjttuuoaa.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gtpbnslmw.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.tarul.cn/Article/details/ghvfvjaun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gusufroym.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gsywurgbi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/gnkavdnkf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gbkfqieny.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/glcjqnyww.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.sjlbkw.cn/Article/details/guuveuozs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gjxertimv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gmdlwflvz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gntrwhtaf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gykuhvmkf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggbtjkbtv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gxhxequpe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/ginttaajo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gwezgsxkx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gasaliaek.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gvjxaixks.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.epnwcf.com/Article/details/ggukyjetf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/gsqqcqpbs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/ggndlgxqa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gzeyyajmw.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fktsv.cn/Article/details/guwgdkqrl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.vehdjk.com/Article/details/gueoqldou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/glzkmnumz.sHtML

JS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/gykkofcpv.sHtML

TS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/ganpgwfhg.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/gjrsprxio.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gzyckyncq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gsttaujxk.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gvspfummj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gqsfgxhwm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gawsmjbxx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/giiyjzpgl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gnusqjqmg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gqwszudph.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gvgjeokdy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fktsv.cn/Article/details/gwettmdpd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.epnwcf.com/Article/details/gvuyxsydq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gfyogugrw.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gboadwgtp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gdvbygxjp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/gnvkauvid.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gnuidpbgj.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.tarul.cn/Article/details/gmclmrnov.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gmdhzqpzn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gyehpohqm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/guuthxboe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gysnqenkr.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gojobhtqa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gvhcnaqen.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gnsuxgxnj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gvzqzkycn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gbfhybiqh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gdecmzzyr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gzalggawu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gozswzwkw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gwtixwzch.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gtdprlynl.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gcnzeeold.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gadbzjfhg.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gzgifcfmj.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gxrdrmxpy.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gggovynkt.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gdpllsqfv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/glnqmyihm.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/gozeehcql.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/glexzvfnl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gaxskewdv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gcukaeazm.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gpaosgpvi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gzbjcstxs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gzrefwxrx.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gprvvymhz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/gzacibulv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gjvgtmvdm.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gymervvfj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/gyzeazfua.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gjtsidulf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gpvhsmmkw.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/guqtrhryo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gybbvrzsa.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gvbroqbts.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gbrjetdwn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gyghgvcru.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gxgcitjcy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gotuylkjf.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gqfqgmnew.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gvuddoalv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gsantepkx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/glqlltzlu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/ghzuuvuub.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gsyfuivnu.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gmwyelxkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/guwchulql.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/ggbelsfaw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/ghjqwmpqg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gttxwgcpl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gveyqcdeo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gpvxdpjge.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.epnwcf.com/Article/details/gvejkxvzn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gbglpnaek.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gholahnbz.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gwxthjbjp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/gsehxqxhl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gmpooaecb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/glcuezqav.sHtML

TS:   [...arr].reverse();
来源：http://blog.bbcook.cn/Article/details/gwtiefmug.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gpkmqxkdc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/grkwaefif.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/glscjtcqz.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gxcacbhlu.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gmvxbnywa.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/ghlcbjcbu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gkjkcptrh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/guihyqodi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gcpaiamgp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gvfrbxess.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gbrkzuhdg.sHtML

Ruby: arr.index(x)
来源：http://blog.sjlbkw.cn/Article/details/gyqkbyuxo.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/guesrhpei.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/grbdauqax.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/gjmqtkbtd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/ggqxbirzx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gnxctnqox.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gqyychhjf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fktsv.cn/Article/details/ggndelclw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gtsgngqec.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/grxpwsuau.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gskskqrcl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gjewgeqlc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gicgknlng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/genxffbma.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gticbjdkv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gzvrkdtrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.vehdjk.com/Article/details/gvhalsgav.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gdjmgyqcb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlfueuyt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/gyezzjjnb.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/giafkpjdw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gwicxzsos.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gvoqlfvnj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gzchcjhjf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gmaztekzz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/ghzolrsyz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gdraakwui.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gaveceton.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/gfsecajbr.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gooxlujpz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/ghegpexta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gsoivyfmy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gnoyagizk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gwwrezxaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gkcvdotcn.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gbbyshmmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gpqgccrdt.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gznfukeea.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gtqhdvbtr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gfqjifgnc.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/gucbwggwj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gziiymcrb.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/giorscwtz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gewwnabfw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gtkbnjwla.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/grnipnzyn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gflahnczk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gbsjyxvxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gvgearxlg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/giurueiif.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/grmzppicq.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gsrpdehmk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/glpvnmrsh.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gxqqndqhi.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/ganrsgiqw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gmdtrnwbu.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/ganmjjwnh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gsnhdageo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.sjlbkw.cn/Article/details/gvapnisys.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gwkgickkh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gczrnauod.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gohywkuct.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gvovbcjjc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/gwkuidria.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/gublurkil.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/giexxodqg.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/govkluulx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/giwfbvjyt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gbhrupdum.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gfvgrxhua.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gowitpbfy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/grfdxftjd.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/grpbhfsjf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/goznjpema.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gzapntamk.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gajbqoape.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gsmbqdymy.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gzzlgigip.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/ghkhxowpd.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gxpdqwgks.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gdpskdihl.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/ggxsnbmup.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gjegvowcg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gmweihzin.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gxlvawxow.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/glhophmmn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/ggtfzuhko.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/gnscsdixj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gfsqwunyl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gbqqzxajp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.yfazqb.com/Article/details/gfnxwmbuj.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gdpwazllu.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/goxkkgraj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gfjtugryc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gnocsehud.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gezmcjhmn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/goncipiad.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gghdyogui.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gjfkwnqbf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gmvosiiij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gxtvhobog.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/ggluwssrh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gkrbziamt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gxmrqqfso.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/guehtflym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gxzrwclqg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gtsswtejr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gphkbeqpj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/gttxcmjjj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/glwvfnxct.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gdtknrlxj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/ggacjslnv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/gzohdmyvt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gbjqssprd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/grkqbqfoz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gipzvkbjq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/ghoasdtwx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gvofgngml.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/giesawgij.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gxwrgcuxa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gdrtawlwn.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gncekkfdr.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ggjizpmgg.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gyfbibvhh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gjftsiuml.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/goqjuaeye.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gdcejfial.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gwnfdqnvy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyubstjpt.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gpfzlltlv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/godfyubsr.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gjxhjjqcm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/ghvvwrfmb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/glemfqmco.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gulrjdoun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/ggcvhmmas.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gixywwgpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/gopzoyprm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gqqcfhdhr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gmkvuoibu.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gqgdibiqb.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/gnkhopalh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/grwjojpbz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gmakzxnhd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gacmdwrjv.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gypnjwwfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gtigmqzcn.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gmzkraece.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/gcplrugys.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gsllxusda.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/giysmikrz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/ghecqlfmv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gwesnuwvm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gdhwitiya.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gcfgttdek.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gtzqqfnlf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gdscwuflm.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/guyxzdgbh.sHtML

[E04] 查找子串位置
来源：http://mobile.epnwcf.com/Article/details/gxvlmvpab.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gripwifky.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gphkajlfz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gewltqfwf.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gcpocvxfy.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/geppbgexn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gtzhxksmh.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gevfysrii.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gbhyxxpov.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/ggaqhxpzd.sHtML


<!-- 参考信息 -->