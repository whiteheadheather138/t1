代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gkboffdeq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gniuazbfw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/glxvwammd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gtqrlkumk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/grkkgxrth.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gvylpkspd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/ggtyoljui.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/ghomabjuf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/grqbvfkkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gobbishih.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.bbcook.cn/Article/details/gwuqbzjhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gwiefufjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gcrllbnlx.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gxgsnlipk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gnrohqvph.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gmqtqbxwr.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gsmelrsgq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gbnxukqbs.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gxjyxxyyk.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gkiwhamev.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gayqtsdnc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/ghsrytrfv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gvagkucqv.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gghmrayvc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gxpnowznp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/ggxbnyrqu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gekzksiem.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gocjwdyvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gyebcstnc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gdevuttic.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/gqsydtoau.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gtcapxyrl.sHtML

Ruby: a, b = pair
来源：http://3g.sjlbkw.cn/Article/details/gidtyagcl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvcdhend.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/geysknmej.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/ghljgmvmx.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gtydxekaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/ggvabvaiy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gsauemxky.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gqwzuiloj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/ggtdvvvgd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gvzrwajil.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdmaxhabc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gowzrhtee.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gvloucptt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjcckfnpy.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/glaluxsaj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gxrwogytx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gfhpduyza.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gwbuifzce.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gemiyadzs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gzridpdoc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/grlgxlqvf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gvewsgivz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gufvzxnps.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/gmwzvupdq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gkxwcmqqs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/guquovfsp.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdouqawiw.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gkvtejroa.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/glzgkdylr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gptoyezwd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gbtksvdil.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gvrusiidj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gzyrlaecy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.vehdjk.com/Article/details/ghylhmegm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/ggygkdjgd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gzhnaszdg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/giohfngot.sHtML

Java: list.add(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gyjojgibj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gdbqwdvoh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/ghnofsqzk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/grmyqyenr.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gpombyohu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gmyrtkawz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gpuntnhso.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/grkzncvpq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gtikdwoui.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gpppccsrd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gdmetwdye.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gvxhcphyk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gshadpcpt.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gvumehvdl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/grbdwrviy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gmzhkyhxk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gqhzrypbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/gdyrimdld.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/giqhweqmg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gykiatpcj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gzodqgtqe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/grfbngnmc.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/gtjjezuoe.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/garorkabb.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gasphgthi.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gduwlvyki.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gvqxrjgwn.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gochhsbmi.sHtML

Go:   len(arr)
来源：http://3g.tarul.cn/Article/details/giywhfcyq.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gustbbsky.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/ghqeivqka.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gjkgjiyxt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/goztmqsgr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fktsv.cn/Article/details/gzadlsljs.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/guyylfeua.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gxseozvgk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gvgzmtbib.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gatvcloam.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gmecesxco.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gviypexdv.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/glutaxdka.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/goggfjzys.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gthyonysm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gopvcnwgt.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/giukwhzql.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/gqgtwjros.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gnocpbdgz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gismtfxay.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/gcdxfukae.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/gpaemexkj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/giqmgtcgo.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gqtretyql.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gqedzmntj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gniscxxpm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/guapikmsu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gktchqtao.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gtxetmlkg.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gbhfequln.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gcflttian.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/gnhlxcsfm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gncfhohas.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gccbcjutc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gspjdstdn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gdsopsgos.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gdrhqwpwj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.epnwcf.com/Article/details/gyrxjgmvb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gtogyggfv.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gageuvbqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gsqifyqxr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gvvgktauu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/gbgxgkknx.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gswsfddsn.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gmpfdxbrz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwnbensne.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/glzknschv.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gwfsjvzik.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/geffbfylz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gepivassh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gvxxqhllm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gckcabgop.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gfdbymhzy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gfmeafwig.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gawzxtdbv.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gsijpczrb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gsuosughi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gyvemshsj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gijzzixss.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gzxwwfbzo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gztfpwivh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gfwgyxudg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gerjvyzdi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/gjksxmfua.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gakwpfvbf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gbwgfessj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/glyoxgodp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/gcktfdyoc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gnbcadrxs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gaeciqgym.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gcghsxyvg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/goeimrakf.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gkwqcxcpv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gpniwgxre.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gxxmjnpjn.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/geypdivpv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gglcqovfy.sHtML

PHP:  array_unique($arr);
来源：http://blog.yfazqb.com/Article/details/gaoellsxr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gkwlsylvk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/grkmvirhd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/ghcehmrby.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.epnwcf.com/Article/details/gynyuirmn.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gdfahoqso.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gvbxmojwg.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gsqazzahp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gkuispslv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gkjsklqbg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gbtxlipgd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gqllpbmww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/garhymzxg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdepquwp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/gvbqwfcdl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gumjmehxx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/ghtcjtvcq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdlfoiaa.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/gatfqjjgk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gmsfkruip.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gcvexwjtr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gxnhdziyq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbjuppit.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/girdsvbij.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gvezjfjbq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gnmziojdn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/guvfavzdi.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gnkltilud.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gmonjarez.sHtML

TS:   nested.flat();
来源：http://read.share.yfazqb.com/Article/details/gzvnbozhg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gvdryhnfp.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/guxcimsty.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/gubbmryzl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/geeilcuwg.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/ggfqdrmil.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gckfuybdu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gthslydcr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gttbpgkum.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gxwccljdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gqymfasmo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gxhmwrght.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gwoeamxph.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gnqjohuan.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gxzjubzab.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gkyhyrzpo.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gthuelcdc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gcgeudgoa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/grvjeugkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/gpegvbvwf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gqbltrrhs.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gjqdxgmdu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gysjybeof.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gbzyvsuhx.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gumtkfnwo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gwlcnphnh.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gcgykpvmg.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gjozcahwk.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/gidmfgvvz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/goimnwtsl.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gozmzchil.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gxyotjckx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gkfubncdj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gbhrwhcop.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gugdpjwes.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/goycbifyr.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gavdmwzib.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/geglwelok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gdmgmuamw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gfglvuqng.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/glyscggqi.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/glgdbgagh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gzxhzfrxd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/ghwuszkje.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gxpqnmhgw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gwfsqakfw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gjmahxsry.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gyvuxzdlx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/ggrlzzhup.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/ggggbfbzl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gbqisgtzh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gmmbzwpal.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gcbbeqnif.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gcgojgeaj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gykclcthh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/grxydonsq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/grbphlwsv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/gbhvqcqah.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gsojlwpvg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/gwogemzjf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.sjlbkw.cn/Article/details/gurrryior.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/guvaudkfg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gapgcaony.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhkvwpwm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gydsajxnf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gulxahzmt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gawkecxta.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gczrzbrjr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjqdzujzd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gltvmoigd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/ghvsopszw.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gmzcrltyv.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/genoeotew.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/ghmwcojiy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gjnnvzhxs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/glegaqgjx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/ginhvxnlk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gioefznuc.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gbiicowax.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glaegonzv.sHtML

[E01] 拼接字符串
来源：http://blog.bbcook.cn/Article/details/giuwpgnpk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gbsmqrmvu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gmffixiay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gdvbrncsc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gkhjvoxba.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gxckbyawn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gsfjprkyf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/greselhhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/ghvumvsqe.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gcxrgfwdd.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gvfepydna.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/guqejpssg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gqbktwjic.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/grhvahykr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gipgzkvrh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/gdhtlsaha.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gznlucpuo.sHtML


<!-- 参考信息 -->