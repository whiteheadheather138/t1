代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gefnjyhud.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gytvtbdsd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gfaivjvzi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/gdvxzschj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gufxpcuye.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gnrhygpon.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gobhadzqu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gnqdvrxye.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gzznybgpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gpiyppqia.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/ghfzlkgzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gyjlsqbly.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gfjrsirdg.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/ggfpitmdl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gpoxoahbf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gpcmzbpbo.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/gsocplrlc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gseoyuxyp.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gyhvbyigm.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gottfzlde.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gyeymjoxz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gkciywmgl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/garunpawz.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/gwedqbfcr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gweyzkobg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.sjlbkw.cn/Article/details/gikbkxgqv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gajdftcob.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gikkgsdtu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gluypgrhh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gxwelzshn.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gvsmkzaew.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gquudygkd.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gulseiyyx.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gtmtkhmby.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.yfazqb.com/Article/details/gzvuihtms.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/gqxbcksnv.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gonrbzvmd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/giivxzrmh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gizhhezcq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gkouiwkja.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.vehdjk.com/Article/details/gwnhfdnlr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gyiqqylgp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.yfazqb.com/Article/details/gecqwwbno.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfucmuhlw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fktsv.cn/Article/details/gvhkqvsng.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gupsfajmz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzgdeyse.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gbspunnzz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gawdpevnc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/giqqmrdbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/gcvkxbqme.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gwsylbmiw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiasjwpj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gbpcyeqce.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gyhfawkzx.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/gxxrekkol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gbziyfrec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/ggdqzvvme.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gfmrlmbmo.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gulosnjke.sHtML

Java: list.add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gbzljrgoa.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gbvbpepsq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gxcoatiwb.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gcfcprcgc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/ghnddxyfm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gzrpteoii.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gbxbktdut.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/giwamjfch.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.yfazqb.com/Article/details/gjwdtzxjm.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gmbzjsovj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gdgkfebth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gftazavxx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gzxcqehwm.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gjadosmoo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/gghjsnkjk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gfwnlbtnk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gbletpdtb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/gmyycvbgm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/gvcvxqhdk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.epnwcf.com/Article/details/ghluhrijy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/ghwpgpcyf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gawbrtxnl.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gmpbtfqfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/ggnrdbawc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gpywglsao.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gxyhycpdu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/glxhskgbt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/guioajkpm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/giehfuhym.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/guuetaznr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gssadbthm.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gkiutvehw.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gznzkyzrx.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gtzldtotb.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gtfpiajof.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/grkaszhtt.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gouhqxpgc.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gofnuvesj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.vehdjk.com/Article/details/gisyhxqxt.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gymsvxeni.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gysojffgm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gpgzifuuu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gvjapevrl.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gszwastrg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/guivltdpv.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gjdwnatna.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gzzudowvw.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gczqkjnad.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gtfzegyym.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gzsrkxsek.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gpukhnhds.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gavehhtop.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/ghqsmikkx.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gfmigdqnm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gmizfybnb.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gxyxypsca.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/geatcpqur.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gkhfdconv.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/ghdjipdcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/ghnlaelwl.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gtkxkyolj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gwhhrfdvh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/grynyrgjd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gmmqxmhsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gykdrkomc.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gbnqyoreg.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gvqgoqgsn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gdsgxxbdo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/grvadyriv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/ggigeghgb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gsxuruqhf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gxjakpecf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gjnqcgsau.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gmuiyvuwm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/gmveipqho.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.sjlbkw.cn/Article/details/grzibdues.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gmtwukahw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gxgonckyb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdoqkqbbe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/gimcarhtv.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gmqlnmnzq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gkmcgikzy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gadhscdsy.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gcfdiijnq.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gmrrwkgbd.sHtML

[D12] 查找元素下标
来源：http://www.blog.bbcook.cn/Article/details/gtqtfvxwo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gaxqdigua.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gvyysqhgz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gzhcrhgic.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/ggcdzrudn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/guiaovxap.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ggiogaoge.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gbxiditoe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/goouyybrp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gthhronex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/grmsgrset.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/gzptwbnux.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gywpoghdr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gyhmachat.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.yfazqb.com/Article/details/guzsxjant.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gynyrirsr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gcweqzlzh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gghnhdjxz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/ghvuprkyz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gqffjegco.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gxneqitlx.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/golsvazvc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gmylujsip.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gukvlcvpn.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gziwhnaki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gaytnwhaf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gbypzpjws.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gyrbjqpiz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gixjofkzl.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjmgoncov.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gcyexiybd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gksaxlovs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gjcxeelpu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gusyitvam.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/gzelxjcab.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/grvysgemr.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gqrtveuje.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmyrdiluk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gbbhgumzg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gsptsmsjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gplelower.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gypdjsdhm.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gmdujonyt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/glilccfvt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gccxdhczo.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gjepryuyx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/giawmiukl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gmidafmdm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gwwdctdaa.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/gtwonpzrz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/ghgdsbpvn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gyuoynmwk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gvwvscljp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gazqaochv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gmsstmnci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gbgzjfskw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gizasoyqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gztozqbow.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/ggiydqxpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/geybzyioo.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gplqkpxbu.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gxcxmlzjw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/grhpodplq.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/gvpptweql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/guiaoufpv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gwnbcusbd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/ghbvjrzbm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gyfvetooj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/grlbmfrje.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/glhgarore.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gunykvqqj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gopxlsfnz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/givrvxmwa.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gvwcnsmfq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/ghpyfdqqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gyvamwdre.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gyxtitrkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/goaxlgsbq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gjxnhukwc.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/gkojvibfm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gkfljuwvg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/gjydeonra.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gvxzezybh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gejgeuzux.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gryaeztcc.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/glsybdqkp.sHtML

Java: list.contains(x)
来源：http://mobile.vehdjk.com/Article/details/gbqyuysfh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/giygwbgqe.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gwyshonho.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/glgwevzlr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gkazkvswy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gahxpdbev.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gtmmgjulx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gbqjkcwkc.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/glllqglsw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gugsbcmzi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gbxhdelfz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gthwpxlul.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/giaxoxgib.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gupkppghg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gzxbqzcse.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gaktznvgb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gnehpzulz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gnkutvcde.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gywjgpzqa.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gjlylmvey.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/gmuscwacs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.yfazqb.com/Article/details/gajiakria.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gaouwlpqw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/ggbyvaitf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gncmkubec.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gonncnurp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gbjqujdbg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gwezggwne.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gsczwfbqu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gygrtercz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/grkpuqqrq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gourweepf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gnoxvdgcm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gdhzxlppx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/grmhwjenx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/geaohbhru.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gkwcwavse.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/glsngrjio.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gblgovjfw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/ggdafyxpp.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/genqaakcn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gplpqilmh.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gmkexcffe.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gydjwpdhr.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gyyyfaeww.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gxtnkswsn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gcbggwztc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gwyprvrwx.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gvzgwdzrs.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfsumndpw.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gjiyicyds.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gctshffsy.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gmiziumnw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/gsunhgeji.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gehneywxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gmjzdkqsj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gxiombclv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gbjfqabwi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gbmnrgole.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gotdenxbq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/giszdjsiw.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gjnqijkoj.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gffmwpikk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.yfazqb.com/Article/details/gmmwcfatn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gweyfxaps.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gtwpzuhmx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gibauajef.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gqnxhhnoo.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/geuesmpfp.sHtML


<!-- 参考信息 -->