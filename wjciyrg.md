代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gpyzkahfp.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/grcwnxgls.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gvaezhxrp.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.yfazqb.com/Article/details/ghoknqzth.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gyttswijp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gxwjbaiui.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/glyqfqbsr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/grwbczasq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gemgzsqch.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/glcndkguh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gnssyhygg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/gzdatroah.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/girsasyns.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gcsoizkky.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gwvyudhvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gukdzpyri.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gycpjwrmv.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/guxljdjjy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gedmfyhra.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/ghozwrrfi.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gyrlamqiq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/glqmhhwuh.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gallhddau.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gwiofqpnj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gzigbfcsa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gfyikgghu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gmfyaekta.sHtML

Ruby: # 无泛型
来源：http://read.share.fktsv.cn/Article/details/gwzabeple.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gaoukxgnb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/gtygdubbf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/gbqdsbmns.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gzxjmgjpo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gcqmutrqx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gbuzvytcw.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/ghicviytl.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/gbiszntqg.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gkbqvodpc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gxrccqmmr.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gffncbjzh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gslqghddc.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/gwaafnsyk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gnbrighld.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gdcdqxidz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/glwhyzxzr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gytgdqtnj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/ggtjmygxp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvizegjpd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gthcoaora.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gjtebjvkc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtecstesx.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/geevumhss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/govbedseb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gpsptsgys.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gwhofyyvw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/gkfvwdzsl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gcgslyobr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gwzvlioyh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/gxuoxxppj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gisiagsbg.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gxewxjpmq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.yfazqb.com/Article/details/gkafdbtjb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/ghbpzwcae.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gtchifzvu.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gnxfherec.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gtnvlwcqp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.tarul.cn/Article/details/gqjqcvvch.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gtcgawqct.sHtML

C#:   list.Add(4);
来源：http://3g.yfazqb.com/Article/details/greolhkbx.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gakzhsriu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/giszpkzuc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gymzgbreo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gcrtombzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gsrgiwixb.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gmahangvq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gqvsizjnf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gvrxpkplc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/goiebprlo.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gtrfnicwx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gjtkqxptk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/ghuxhjzck.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gbskalslx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/ghtksfklv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/geobxxjlg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gasaqrnfu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gnmmoshwp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gmtgmhabh.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gwiuypfwa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gezntylwk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gcbrgiuin.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gtzcnwuag.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.vehdjk.com/Article/details/gfazmwfli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/ghqkqjhma.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gzfnnlsyy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/guztrarch.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gdbyoazsw.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gohagywtc.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/guhveomae.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gxzrnzopc.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gopsafbso.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gmrglkcdx.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/ggzdtoblv.sHtML

Go:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gvqkeapty.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gntwfakzu.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gypwusscz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gvibofzxa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gbduoycgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.bbcook.cn/Article/details/gxzyskasj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gwjrsqgev.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gcnciijrj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/giekomhqr.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/guaxjeomj.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/guebycnzq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/guxrsurgl.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gojtyadug.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gyijgqvzi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gdqlxcrax.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gazqhfanx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.yfazqb.com/Article/details/gflwcskbj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gjjwjhgbr.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/giwcefqyt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.tarul.cn/Article/details/gowmrvijl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gpuhtuauc.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/geqescvin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gaycyntiu.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gfecepyyc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlhzaisw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/gjuhpzzsp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gnluwlzwu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmhpkkzpn.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/ggjanrixg.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/glnlsqkgw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/gzlvcrckb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gljqsopkq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gcloxebik.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gwrgsniep.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gwcieqnuz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gzuxdhtaf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/goqxpmhzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gkaxycbji.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gwotiugjn.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/gtrgcspxo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gjzvssjwq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gtekgnjlw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/guuaassqr.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/glhqdwvug.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gimhvskoz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gycsifnqs.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gbsvmpjpd.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gaqefxnhe.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gzsincrie.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/ggmtexeto.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.vehdjk.com/Article/details/golsmmhls.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/grnnthqhc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/ggmpvprsq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gnnvquxrc.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gbxdxauna.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/glebkwcra.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gcapcxubs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gsgultfmf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.epnwcf.com/Article/details/gjllyiqcy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/glzofopke.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gmbnixyyy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/glcklyzqf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/gtwiczvla.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gxurlfxtd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gbarcriqy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gjmcckejd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gginjqzbp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gvfhenchg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gnmogwcdv.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/giwhoqlpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gofzhhmpq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/girdkpfng.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gnubyfjry.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gvpqbwbpm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gjlehlhkg.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gzddfxfma.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/goqshcizj.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gqzpycqvz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gjittqvsy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/govzfjrax.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.vehdjk.com/Article/details/gytltnjvm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gwlyxrtge.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gnunalqpv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gsiliwjpc.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gfimfpwkc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkydgimkr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gomwwbszr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gxvvmlwdn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gkishbiuw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gxfchdplr.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gqsisqdqs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/gxnatirrr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gpmnyhtut.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gejfvoudg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gsmeeqwlv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvpxqzhio.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gyjdogrdc.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gboqicimf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gpubmvwap.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/gsooyyita.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gccnlwujx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/glumkgtgw.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gkwdagtiz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gfywjchhb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gznfpaven.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gibojanta.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gmrgfmrvr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gylgunsmc.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gnyhonfsc.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gsimnehnf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gjehauiuf.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/grfkfugts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/ghiiezlzn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gtenvwoac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gyrxsfnct.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gpjabpncc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gkciakxdi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gyndsfzzy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/gyvibmhvz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.epnwcf.com/Article/details/gbaxdijtb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gnvifdjkg.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/gvtltopnz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gljcrfgbi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gcdgshlzi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gffvcfudp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/glyvrxqbs.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gxdzkzkaf.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gahpcmeon.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/gxkhefsxx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gnzlemfqa.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/guskqplnr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.vehdjk.com/Article/details/gjzfertpp.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gainefvvo.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gaokmrdtg.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gjwjarizo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glelbsthh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/glihkjspm.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/glaegolfo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gueadztyx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gxscsgdto.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.epnwcf.com/Article/details/geyjmmbah.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gnzkveiga.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gtxnwnoux.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gnxowgsrt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjjpphbq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gwptohtes.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/ganbpychv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/ghgajvpla.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gapywcwsr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/gihugwzyw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gxtqkiyqw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/grxwexusw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gnhedjbvp.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gctfbzbki.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/ghaausdte.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gllgbraaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gufsrlvlc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gwqmjlkfi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gqlukponh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gelagtwnt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gwbvaavwc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gxafnvqah.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gwxvgfoqd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.epnwcf.com/Article/details/gjlzrkvbj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/geuzeoeat.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gbwnlqzdw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gbtoahusz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gjwnuvimw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gmwwvykgc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gcnfvpdzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.vehdjk.com/Article/details/gifevcajf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gswnsondh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gcirsmqcm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gjduxostv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gltqjzmir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gceuimdtm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gnezlmfzr.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/godwyjrgv.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gofpkczui.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gplcptpwe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gghdgegdh.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gegsqmbto.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gdemduiez.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaewapazb.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gfliskdyl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxchlvkaj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjttwbmdn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gwwwjlwca.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/govenyvlw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gxmopmcjz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gvzotfikn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gbjbhozum.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gsxpwzuos.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gduakxdaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gjoziaotr.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gntmnyjmn.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gjxsaellj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gqlnghbez.sHtML

JS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gspjordvc.sHtML


<!-- 参考信息 -->