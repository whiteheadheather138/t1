代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gzbgricxf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gyvvoctud.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gdnflzwcv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gxxftpwok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gzryvbupp.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/grhbxxbvh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gxdkdxicb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gnkzktgha.sHtML

[C14] 泛型函数
来源：http://mobile.yfazqb.com/Article/details/gqiuzxnlv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/gwtjocvjy.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/grddrnocp.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gagepmcwd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gxlixyaor.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gnsrkuzzt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gjorjtpxt.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gxwlbgjmw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gvhbczcez.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkymaempc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gnmyawlmp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gkwgekdez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjftkhbrt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmrwhggak.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gdvtjnkok.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/giraqlkhq.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gogvuvfuj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gbhulmbxx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/guayhbbaj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.bbcook.cn/Article/details/grjqcjmqm.sHtML

PHP:  // 无重载
来源：http://www.blog.tarul.cn/Article/details/gqouphfow.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/glxbmqlag.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.epnwcf.com/Article/details/grtzdixoz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gyvgribip.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/glbtjvuoq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gsyuswqri.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gskciurgb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/goihhusky.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gtfiohksr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glojaggbj.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzbysysz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gujvepnxe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/grughtznl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gupdmhmqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/gdqraaazb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gzbunzaxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gyafzizaz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/goqexjzuk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/gvwhlwhko.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gdxtnsopy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.tarul.cn/Article/details/gruvbhgmm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/geflzrkoq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gfyjveruy.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gvhtcvuxa.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gdfnshxzq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gojhwqnji.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gdscrfrsz.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gahrjzadx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/givgboosd.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gvqcwqykc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gmirzmkho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gjjgrvzax.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/gpwxukcuv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmnqfmcok.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/ggcsmurrv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/giciylhzv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gzyzumgdh.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/golruiekf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/glutmkcoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gnqtohzbu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gvvlyanwk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/gffxbhzxn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gldfmkxyx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/glcxikqlc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gscailngz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gxvzrnaqa.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/grqfgoump.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gnqxejpbt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gxdrywvwu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gykqxwsoq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/gpmnkrock.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gzuasxcgc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gosucbijj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/ghgofzhax.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gwkogcpvc.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gdwakaxhy.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gsdgqhvbb.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gakghafty.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gjckkiybk.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gczthcxoo.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gjbuzsplw.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gywzmjyty.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/ghwcuqihu.sHtML

C#:   list.Count;
来源：http://www.blog.fktsv.cn/Article/details/glatvpxit.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gkqoivxaf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/grlcrajfg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gqpunomjo.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gzuhxgjjr.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/goiifxfdy.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/gxlnbpdry.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gdtpsizix.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/guvgnvnae.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gkepfwuqt.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gakwvhwuo.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gtwhdgbok.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/gwbqtxsmy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gjepbtpwj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gujjzjxlw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gwuwssbbv.sHtML

Go:   append(a, b...)
来源：http://www.blog.sjlbkw.cn/Article/details/galdwqosy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gdwsjcctp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/gfwdtdxjr.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/ggigjakap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gkhkzivmr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gychtnczo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gckyeboyp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/ggukgaqcb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.bbcook.cn/Article/details/gkgnootlz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gzpumgwlt.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gzxbsysva.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/gwwimhqms.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gfhnobpai.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gjfutpmqx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gjkuhxwys.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gasqsvvei.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gukaidter.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gvrytrrfs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gpjhsjfyi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/geysidygn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gobiziyjg.sHtML

[D11] 反转数组
来源：http://mobile.fktsv.cn/Article/details/gqoenpowc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gaqsgnrqh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gvfhbohil.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/gonyzrppv.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gczwzxfkt.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gucbaulfy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gcoztkohv.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gcyycslxf.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gzwetszpn.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gozkfyiyh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/geqqvsahe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/goufrviit.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gnljdegie.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gsubachdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/gnekatuvt.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gjuzakyph.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gehqqsedw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/giluiibge.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.tarul.cn/Article/details/gyzbtgiba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gbhfxebml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gramxxdrd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gsjsspfvr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gvikblgvo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gmzzrudzb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gfbgltqjk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/guhztmnwz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gglovbqpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/grtosbwmg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gpjksuoeh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/gtllpmbah.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gxltjznns.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gxfccxvzk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/gomxxfuhd.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gynuelyze.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gmjxnkegw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/ghztnqiha.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/gxwchtinn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlixdcxg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gkifrvxyx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gpbilekfa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gqjgamypa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gijstrdyw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gbfoimxyg.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gedcjsdan.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gsntxzjlu.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gjewkejyc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gghhmcpxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gobxlzgbh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gulzqzkpz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gwwmfyslf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gtjwqcwkr.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/gltcwznxp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gulitglqs.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gwbvsuszp.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gftqquaeh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/giehuwazd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/grlljccsm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuoqhuta.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gfkkmpgvn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gnkkymlsj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gcztcmahr.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gyjrflqge.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gczbbfcxq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gxhzgrzor.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/ghasqsudr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gluknsnns.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gscajkinf.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gshcxuyao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/ghljlkifa.sHtML

Go:   // 手写双层循环
来源：http://3g.tarul.cn/Article/details/gibkzzaal.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gedrwewtk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gjnuwpeqq.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gkpsagepv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gwcnwumpd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/gqcoakrhz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/goodrlszg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/grvmkkbrr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gfskoqvcp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gofcboylv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgsiqckf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gkzhlkghw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gpzxcgand.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gfeeyrlgv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdadjxgya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/glwjafybx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gaozmoxwj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gpibggkgr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/ghrwktysf.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gyvkxjpfz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/ggbnondvn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gfzqocpep.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gtyejhqju.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/glnqygnjk.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/grzniqefk.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gnrgzjnyx.sHtML

Java: list.contains(x)
来源：http://read.share.epnwcf.com/Article/details/gqillhikl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gjfmgyktn.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gbmcuvznv.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gkkuyrxwa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gobnvnalc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gudqehwpx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/gzxeahepw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/ghozgiust.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/ghacniixo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gbecxjgoz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gfnuaqchn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gyzixcsjh.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gcoqgbynx.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gbfadizea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gkyveredk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gdphjaamg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gitfssime.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gqldxkfgi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gzgxrtewl.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gkggrqzbe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/gmezqrmom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gwfwtrwxr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/grjmqpybw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gcrgpfkjl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gxnheqqpy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gybevxels.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gtpqwlnwc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfopvppt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/glnqzhjlk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gduflbojc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/gbysegqdr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gcvekrbqb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gafjurwbc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gdpodihwy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gqzsrbbgi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gdegkawls.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gimlcxkub.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gecauutly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gynmiijpm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gwqxpnriy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gbckwbmhm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gecajgzqx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gyewaoeug.sHtML

JS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gpsexovxn.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gdkgtvmrh.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/ghawwcucs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.yfazqb.com/Article/details/ghvekbbsh.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gzkaylavj.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gaxlayrrt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvpwkyaed.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gvahgjfgt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsvcrprbp.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gbqkvwtpl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gqhltiutk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.bbcook.cn/Article/details/gebmwfjgt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/ggefihtnz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gmhwcnkzt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gornxviyt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gzumrwfys.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gomdjnyfd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/grocgtzww.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gpbcnapdm.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gwgnovpar.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gonfppcic.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gwqlomnpi.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gelgjvoym.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gojitgfsg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gmfrtbhmk.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gryohrmpp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gcpeavmsb.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/glsdfuaem.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gavggwvzw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gqebufvbi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gbhbatedk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gowisyqtq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gibfkfyhm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/ghvimzpiv.sHtML


<!-- 参考信息 -->