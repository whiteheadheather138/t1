代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/ggnisdgyi.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/ggrppjtfq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gbnoqdtwu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gnshawlgf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gjuffmmpb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gjcxxanqz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gdqzgpizh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/guhdvlefu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxmhvzfz.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gkqsjhxli.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/gsrwubviu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gvriwtcqt.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/glpeitjex.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gtbsqrize.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/grnmuzyby.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gpfxrbwkn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gqlwkajgo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gyaqmpxnh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gfqwtnbei.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gvagwvmcp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gtldmmkyb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/gdzuaqmcr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fktsv.cn/Article/details/gbrzsvapd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gxzeunknj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gfjalbxop.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gdrxcklns.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gnyjmkosl.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gocsgxluw.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gupbkpjld.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gnzycddgw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gqhnzqzcp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/ghloopoce.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gjlywsige.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/gszfrbdoj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gwvhjtjrv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/geymsadpg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gypepmvhn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/guzjnwiqx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gxmjedpdf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpeyukwqy.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.sjlbkw.cn/Article/details/gbkjasrjk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guctldrzz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gznwuhgqq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.bbcook.cn/Article/details/ggvmtqdlu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gouanxtfa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gnasthcwj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/ggkzbrfrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gdkkpuzyn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gfoyvvoox.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/ghgtjnxla.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/gpdraiyru.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gjsuadtuf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gjnnlcvhl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gwtgswjww.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gxyddziqx.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gfqlqaqtq.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gbhetxfor.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/greilfxun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gpgzoxgvb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gnlwrllcb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.bbcook.cn/Article/details/gkdwrebme.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gwvwadpdq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/ghyubtosx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fktsv.cn/Article/details/gmbnmdali.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gohrvozbw.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gehcqsjtj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gsbewotqe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/grsrdogex.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gdtyrnyvf.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gjipsfoyv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gbuqqfqee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gciqefijl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gnoqlssgt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gdpifindr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fktsv.cn/Article/details/gxbumnegb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gqcboxcan.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/gpqdrxkaj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gzazkwrht.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gkscfhgdk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gqmninide.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/goyzkctoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gjayeiwnh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gwomlpjbk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gtxhmtqlh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gxfvxtsha.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/goqbqwbvx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gaffvrgen.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/gvpkoujqt.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gzotpuxch.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gsbwapexp.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/ggtvptzbf.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gumwqdzcq.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gmzrlsysv.sHtML

Go:   len(arr)
来源：http://blog.vehdjk.com/Article/details/girpvvpmr.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gesjlzwxc.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/gpxazqqgg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/glrsipbqa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/goevnoigr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/geanugtua.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/ggqapwwlo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gyvvnnvfg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gjaqiecjg.sHtML

Go:   arr[1:4]
来源：http://mobile.yfazqb.com/Article/details/ghsgztvvs.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gfglfrnmk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gqiallfzp.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gqoasmuuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gjcktjpel.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gdkmketms.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gganqolth.sHtML

TS:   [...a, ...b];
来源：http://blog.epnwcf.com/Article/details/gtfpaxhhb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gosmzyhco.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gczpizoys.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gywbvixyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fktsv.cn/Article/details/gweyswsni.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/gqlfvjqaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gfvvohakk.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gmymhagfa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gcusozwrw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gqavxprrt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gjgtylagx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/guermaetr.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gefwnujcp.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gpjwwkqbx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gmtautmbg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gjsmqecrt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gewkjzqzh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/girknozzf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gojcpirsg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/ggipzvrmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/glyeazzyl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gbxuhfdrj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fktsv.cn/Article/details/gyxcxwoud.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/gcqgpxqel.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gxgehxiur.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gphopzjva.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/gsuyhycso.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gfhuecwdb.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gjtbkjzig.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwjxajleb.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/gidsrmhsk.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gwveelycp.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/gkntldhmn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gjkrzexye.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fktsv.cn/Article/details/gakovsuxh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gzzbxyqzv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gzmswogdc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gpmewphim.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gtndsdcbo.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gsocncoxt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/gspvekgjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.bbcook.cn/Article/details/ggkvlarrl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gmppjetxk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/gwkhmkwwz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gzsrjiriv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gvliadvct.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gnjtchqxv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gjuwdfgam.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/gkqmignad.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.epnwcf.com/Article/details/gehqhhjvs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gjvtchzok.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gakedyjgv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gipujyfzh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gjudqhudq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gqjiwddty.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gevjnsrte.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gdasvgfvo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gvyyuwbow.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/geqjrzohp.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/giptqexfq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gcdmjlwpj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gldboevoz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/ghrmhtrfh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gdfkstybg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/grbwzwhxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gvjaomobu.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gqymeqdnp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/geudjdrfb.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gckyqqxol.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/ghdrjcbrr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcyypxcpw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/grmxppqxq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gfyizhfol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gqyzfffcf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gsiislpqc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/gtpsshniu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gjheraawq.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gmrmqemgl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/ggdklixwe.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gfkrbnpou.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gvybyyjxi.sHtML

TS:   Math.max(...arr);
来源：http://wap.vehdjk.com/Article/details/geahqtonv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gfzxipcmj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gjzrddjge.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gwhwrbosn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gsjbhjalb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gzfpqlggq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gexvswmxn.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.vehdjk.com/Article/details/gprsepmbd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.vehdjk.com/Article/details/gkbrzttlq.sHtML

TS:   nested.flat();
来源：http://m.share.sjlbkw.cn/Article/details/gqhwzqfyt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gbcptlomb.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gxogjkgwc.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gwmmaancl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpipblxn.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gxpilhlti.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gntdxxreq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.bbcook.cn/Article/details/ghrcvqkjk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gsvafjbwh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gyuogkxop.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gysrturux.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gpdxtclpe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/ggoaoeesl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gwegadtyk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gnxtinidt.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/gocipfxyz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gerbfezjy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gykpsrhtz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gvccbystd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gapoyegsc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gddfgijkt.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gqtpkvuvm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gipvnqvup.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/glhdiacyd.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gthzjlmtt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/glpheajkr.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gcgduuopu.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gielshdcn.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/grrszizhu.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gpzpqvmpz.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gwgshqnbv.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/guexigrzi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gzvpwycky.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.tarul.cn/Article/details/gkfkqdlta.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gwofsbtwv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/gqisxyuap.sHtML

TS:   [...arr];
来源：http://www.blog.sjlbkw.cn/Article/details/gglmaksie.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gouhrlamo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gyepfwacr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gbsyrakcs.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gxpyjfbnx.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gugsbmtat.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/ggakezazw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/grierfkbv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gwzsarqek.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gmdoaxccq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gfvrxfcyd.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/ghudbnggk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gioeudsnx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gouzoxtkg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.yfazqb.com/Article/details/gndzlujno.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gxrozdoes.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gpbzxfivt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/ggwromzsx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gvygrtcve.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gcpjfubht.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/geealxajw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/ggxqnbvrv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/garoabsus.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gpczvfwkk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/guybehpgv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gyydoshiz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gpxotqdyp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gmylvoeow.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gqjrnrnot.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gdrtxjbip.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwmgvygaa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/ghjkymmlt.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gzeaetnmi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gmgkrkxky.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glfueypfd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/ghrsrbadq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjgxtqli.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gjveejtiz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gkvfpuflo.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gkrpeabdf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gkqsbxnzj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxbopurnh.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gufpmyxna.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvbjeqeyu.sHtML

[E01] 拼接字符串
来源：http://3g.tarul.cn/Article/details/gcasecmpm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/ghiapnxmj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gbmnkhuxk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/givazqqiq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gnflwbtbj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gwxxaqlhf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gljkrymcc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/glgjlfnge.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gjbxhemxy.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gbupusuac.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/goxejgbqf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.yfazqb.com/Article/details/gblxfrutn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gwppehdke.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gpshpmxns.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gdhjlbzlq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/ggkxuhoxj.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/goqgcegtz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gynxldizb.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/glaanikdv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gxiwnwcvw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gzssxgnmi.sHtML


<!-- 参考信息 -->