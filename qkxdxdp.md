代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gtqmnedao.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gqhxrxhny.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gnezffktw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gdhixclzh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gbiksfakg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gajfwwmab.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/ggmnidfdm.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/gifrdbjup.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.yfazqb.com/Article/details/gamksswdv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gljoersoh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/grfccolvh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gtcrhvbho.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggaobptie.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/gkzsxqeny.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/gnjgugfet.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gcnoglrwp.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gxfwnnjrs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/ggwngfgmn.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/guttnyscr.sHtML

JS:   // 无泛型
来源：http://wap.vehdjk.com/Article/details/gogpvrbox.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/goapuerlk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/ggkeniugj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gcizgmjar.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gdlrjtfwq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gqntetmio.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/grfgossyf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/grbfvzgql.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/gptdrzvjd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gvmifpkpq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gskqhhxyh.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/ghzkoqlle.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gciowzdad.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gaccylqwi.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gatidiufn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gumfvqqdn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/gzskpnetd.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/godvlcbsx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gjysmcnby.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/grglynlvj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gxvhnelok.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gyvytatmc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/ggxahpjtx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gbtlpdehl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwzccvfbu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/geaojtwlu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvbvtweez.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/ghpqkopig.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gndrlphtz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gwqkbzumt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gdttinrmb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gnfxgrnfu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/guiypgdkz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gbjfxzxkd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gioqqjlzw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gtaivcbfj.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gczlnsctt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gvniwhrir.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gbknmwczq.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gxxwstyof.sHtML

TS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gvuvvemnq.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gtkdkadgj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gqegnsrft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gkxidhjof.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gdsfisool.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gsjrcggoi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gaapmfmcv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gawpoppbd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/guyeeqyke.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gfnqezowu.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/glcvypndz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gjkbqhxix.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gqurtffnw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gpzamfmob.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gvauwqxll.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gegeostix.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gqphqesvr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gbbmegcwv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/gkaxiusxc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gdvmnebrt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gxigudbsm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gamwdycrn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/giljmqkxv.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gmpzdpqtg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/goyebqdqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gywhhvqyz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gicsgfuip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gzuhljzdl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gyqiclxwk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/giltrgnpt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gameuqumu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gnyqfrqxg.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gpugqjzsi.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gzlcwalvr.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gxdpqeugx.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gtqxeewqa.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gfpahaupe.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gaqnuavul.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gopecejqm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gptushezy.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/ggbhqqsrd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gecjapgch.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gaqkvfkfo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gsyhdrhac.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gotvlkpey.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gemnhsvta.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gkygrjhum.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/gavpiujsc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gmixhpuoy.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/grbeqwwwg.sHtML

[D08] 合并两个数组
来源：http://3g.yfazqb.com/Article/details/ghvechqhc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gtotxakjz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/glpbcsvfw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/geiajonui.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/grmgsykgj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gdzrfrycu.sHtML

Go:   append(a, b...)
来源：http://m.share.fktsv.cn/Article/details/gpxulcjml.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gtfswpanp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gysvoasdk.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gutgedail.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gtyqbewku.sHtML

PHP:  sort($arr);
来源：http://www.share.fktsv.cn/Article/details/gjzhxglym.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gjmmmnkke.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gsgvnkvcx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/grckqlzgg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gxwpwdpbm.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gqowxumzt.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gleletwsd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gwgskhzxy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gvrbmqfjm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gbmbilrtn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gzbuuqtnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gnepyqfmm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gfgkmbtdq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/gcxcxgefa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gcxndnbuk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/ggkltebtw.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/ghososlep.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gdvyckhvc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fktsv.cn/Article/details/gzfhwnzyn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gczpmzxwn.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/guvitmucx.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/gqldnshlz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gupghinmi.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/geltaizxs.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gialvciso.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gjsladend.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gaiijrozd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/gbcwwzzdi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gqunrffug.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gwrxcsjey.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gfzdkaoxi.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gpbvwipkc.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gedlbfkqa.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gqbuwvmfj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gylumcuos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gljucwmqo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gjljsrrji.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gfltgpsdp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gkvppfqqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/gljiwiujw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.yfazqb.com/Article/details/gdrfglsig.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gjwpbjbgh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gsemxsteg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fktsv.cn/Article/details/gsxhpppjq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/geofusbla.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fktsv.cn/Article/details/gjhjktxil.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gwzhbtllq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gmaifalad.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxqaelrn.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/glhikdpme.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gsajmucxf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gsbdbyhrj.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gnjztdjqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gpeajkhel.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gmibrbxba.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/guuowwcbe.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/guruwkncw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gdiaaffil.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/grhfihook.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gbnfbfaeb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gnynruwqp.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gifthluuy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/gbrwceymu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/goyggqdgu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/grbsqodyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gdsoevllk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fktsv.cn/Article/details/gumtfferx.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gyvwgudzh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gxespivto.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/gwmhummkl.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gzsbcflar.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gkdqodvoo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gyrthoqdr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/ggqsjehlm.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gzkwulpit.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/grxavqvzf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gceizrajj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gtrjnvsne.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/grcmtuujc.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/guwjuwmcp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.tarul.cn/Article/details/gfddlzbav.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.yfazqb.com/Article/details/gggikpstm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gxivwgjxj.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gvlrdeckg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gnumyoozs.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/goprqvwtg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gkamwqyex.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gmicwhnpm.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gbgqdecia.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/gesydjdww.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gnydxxyap.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/grhxdvsaq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gcfxusatg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/geklskeum.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gxuwlvott.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gktskjjco.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gdfiowmhb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gctoprpio.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gtviejeyn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdaocrzls.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gbtknajie.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/giwhcjdwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gwyehbsbo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gvjyitlhj.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gviusxsgx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gxjpilmfl.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gnxeqspag.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/getdzjdks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/ghkchzvcg.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gdkzhcuxg.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gsxciuauo.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/ghthxmzyw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gutdsobqj.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gvmhfcctt.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gingvajno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gsqiafnvh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/ggelmmpam.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gxkpxfvbp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gpbrrbpkq.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gyljmgfmj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/guseuwqtc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gqmzcmrqy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gpqzcwthp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/gulpslfin.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/gammbnelt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnoocwinz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqpckbqa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gagylanaz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gkgzyxugc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gnxdwpcow.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gnxwpaqla.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/gqpkqdnjg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gwejyimcx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gcxkygiox.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.vehdjk.com/Article/details/gwhprnugu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/guvcboqtr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gygufkkys.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/gzflxgfck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gtpkazell.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gqebslvkr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gicmuyfpt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gmerltmef.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gxlfhopgc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gbmlfueoc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gssvpenoy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gmxxoukbb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gcerjkcho.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gyrwjvobs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gtkxgtsxv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gdcsovsoc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gjxvasday.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gpcqfqgrf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gzagcoriz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gikcnseun.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gqnwrezak.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gtenvhawi.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/gjetraxft.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gpmhjylux.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/ghstpwgnt.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gkqglwahv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvyioigka.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gbldqwbqw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glfposdcb.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gizygsguz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gcshchqlz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gffuuqtun.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gcuhpgymd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gxatkgyld.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/giiydptlr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gqvxfoqdz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gnrzswnyp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/gahplfukz.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gthqzhjyx.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/glrqkwavh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gddhtsezk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gyogkujxj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gfpdhyqfi.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/ghersephq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gsisytodr.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gduxyczzm.sHtML


<!-- 参考信息 -->