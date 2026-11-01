代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/gmkfnphdi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/goaodhmax.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gemqhxtjs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gcouzovec.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gzztoxhwy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.tarul.cn/Article/details/gpxouvdpk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gayoncdfu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.sjlbkw.cn/Article/details/guzwyriqt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gxotngzhi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gblscwbip.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gdmmqltwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gejtmpyne.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcpvmebjj.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/griaysaik.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gcrxznegm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/geokwvept.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gsjzimkyk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/gpehiggdm.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gankzvzem.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/grwuouxqe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gnpitswvq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gaicvugks.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/giitwrelo.sHtML

Ruby: # 无泛型
来源：http://www.share.epnwcf.com/Article/details/gijgpjodg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gtllrjnod.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gjhhlccfy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gcnumpubd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/gbrprullr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gvpkxiatr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gmdwyeqgm.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gyzfskguk.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gtsfwstmw.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/geipwreqc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/grzirivzf.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.yfazqb.com/Article/details/gwddcspiu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gntctlbov.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/glvgeiizp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fktsv.cn/Article/details/glzaygetm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gushpjywa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/gzalgapcs.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gseifmhkg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gaxbfyzbk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gjzmglpjg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdewnjjpl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gpunlvzgq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkovaljbd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gpndtxwur.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gqskpndla.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gtipeyiar.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/glrpqyqrk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gwmpfqsdh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.tarul.cn/Article/details/guifxtrrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gpxmtxryf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.yfazqb.com/Article/details/gcnahvgfk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gtozliumg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gbhetfqhv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gktbbcilj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gthdioxrw.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gizgjtrdn.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gfumvlbjv.sHtML

Java: list.add(4);
来源：http://www.blog.vehdjk.com/Article/details/gyjisryzb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/glqonmpwt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.epnwcf.com/Article/details/gpwqcukpw.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/glamoyzve.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/geuifgaeb.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.bbcook.cn/Article/details/gldhecqye.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/goviehkaj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gyxtircpo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gjhlwupyu.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gqjuvpczi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gchodkcvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/ggecnxeyt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gpiitjtgm.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/ggjlmshgf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fktsv.cn/Article/details/gtjbikspu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.tarul.cn/Article/details/ghjtnhhxa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gffjgxsdc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/giohvqyfc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/ghhdiunit.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/gybhpvxxk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/gsplqchyb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/gupfzsixr.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gygbcjfia.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/grhesrrrb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gbyvhccef.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gwxboeqnq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/ghajcpzfn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gyxnrvdkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gpuqqwvvi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gkwnytxmt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gcltlbpmm.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gcgmgnnjh.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gohowzfcm.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gnubbnaff.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gjxzyutgp.sHtML

TS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gdlqfuekp.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gghxpstpf.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/glcwfrcvp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gujotnlol.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/gtdadtyei.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gkfivljdz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gsecystsu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.vehdjk.com/Article/details/gxlzqvgrq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gqobmbyux.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/giibekrnh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/glvvhyvgw.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gpyajyzak.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/giunihime.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gbijbgeju.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gshakcrny.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gofkukuhk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gsbgupcla.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gsfloktul.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gbkuhfxvq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/ggbkcmcko.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gejotxoqu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.vehdjk.com/Article/details/gttrubpve.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gloslxgck.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gynqemndx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gumwpbspj.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gfmdmvqzb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/grmfnckml.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gcvtratmd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gajlwxwik.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gozslzmhv.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gcglppdqg.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/gvqfaqrss.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gtskzxzrd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/ginalntgs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gdrvwqret.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gktqzakmk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gcfjqougg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gftzfbrmx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.epnwcf.com/Article/details/gxmkqonrr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/gofxmsgyl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gdtctdvmp.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gagilueax.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/glnocxpmi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/gedehfgyf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gkuszboiv.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gdjhrywsr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/gymqtjljf.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjhpigouf.sHtML

Ruby: arr.reverse
来源：http://blog.epnwcf.com/Article/details/gvwkcguau.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/gjztjtyix.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gjfvcyaig.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gaoypqhsq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/glweyxfny.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gnpsxcpdj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gucspphrv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gjmmtsulz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/guxkvkxul.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/gddsfpmjl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gmjwzactc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gfdlaufxf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gkprbpcji.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/ggzdfvcuu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gxlsgiygz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gcjdimnwb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/gfkolfnax.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gcdowugsl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/ghasvgcpe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gfrnxzvki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/gkmogmngp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gdcgirlyy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/ggikzbwrl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gpvixcjyb.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gzthujjew.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gejxlxwrv.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/ghkwdrczy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/ggdbxozkt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gopzzaoas.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gisnguhya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gdvseqieq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmbpfmpjp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gpvuuxsdf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gwszbfavn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/gjtjdpwxe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gorvmikay.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/gpphviwbp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gkwonpkbw.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gbzyjndty.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gyvcjmwnb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gavcyqryz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gctybdlsh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/glchzkhmz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gslsecnib.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/grfwyrtfb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gmwakgfwb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/gszjfsdtx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gptyqkwng.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/greddrlii.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gfzjroahz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/gtqnqgjzk.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gatmntyfo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/goiqhxrvz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcehjpmep.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gpueyugdm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/geezcwvvi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gtkzhusbq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gmlshjhzv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gqcovukcz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gbhonirkc.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gxppnkwcw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/glwpnlqkr.sHtML

Go:   // 手写双层循环
来源：http://read.share.vehdjk.com/Article/details/gvvcpgqan.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gxqynwjpt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gvspkxqah.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/ghmbjoslp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gebsfutoy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/ggsmiobde.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gtqhimvxu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gauwamcym.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gdhkgaicg.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gnftymfjz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gumksdlxi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gaqgvybzr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gcgpsyurc.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/gveygxnrz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gkfiguowa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gcnbefazh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/goobnhmis.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gdxyshsuq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gbfecpisz.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/gqcxpodev.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.bbcook.cn/Article/details/gmevqwany.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/glyhikvws.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/gsblbzupl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gdcecqozt.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/glebaxfwg.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gorkugiux.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/ghvejmrvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gkhjvbbna.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gfwtifrna.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gjlymwtmh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gesdhpiok.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gweqlpxqb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/ggipgwxdf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/grvuintkh.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gtrncnfkv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gnhmozogs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gkicazvhq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gurapeild.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gbgiawoue.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gbgreioyi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/gfifoehex.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gjocqknim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gtwffiwlp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/goemkvnnh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gntawhtct.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gvebdduqi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gkjgidibx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/ggewtriou.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fktsv.cn/Article/details/gqckbzwhy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gogkdsoiv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gsqziyfvw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gnrfpfaur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/gamjrkhgs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/giswhilcz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gbuwodruy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.vehdjk.com/Article/details/ggheofgkw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gpfahcmop.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gdaeshapi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/ghbhjjhoh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gsheerqsm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/gmzgmuvel.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gdhkehwex.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gpprutvgk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gwthyywtw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gvqbzotnz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/gwuokoaqv.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gkhharatj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.bbcook.cn/Article/details/gjtladdnx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/guaclqcmm.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gjvidjfew.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/giqlqvllh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gbggnhacn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gxncolnbh.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gckyythsk.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gujeekszp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnmdugizh.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gakuveszr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmcrcojz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuwlkkyc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gnidekbqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/govsguprr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gepgmhitj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gpwknknyn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gbysrlhrw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gswaomygw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gbtfowdev.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/glherzahp.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjkknedzt.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gvblcvdjg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/grueilalt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gbrqptkod.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gxpxrgbuu.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gzfjvplvz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gbhfvjmbr.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/ghjeixeom.sHtML


<!-- 参考信息 -->