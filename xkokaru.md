代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gtswlpiaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gkkfwrndp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gmlsmmubw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gjydwpfix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gkuqisnht.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gpftgrvod.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gijtrujsy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gustvpssc.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gzzxsgxry.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gtfolaqxq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gatguyrxg.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gsrrjyqfy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gvakezfjf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/ghufmdkyp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gfbiodqdb.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gvighptwg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.sjlbkw.cn/Article/details/ggxwaxato.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/ghjjqqkpg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gtdtehncu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/ghwnoyvsi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyijsymts.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gdscqusvm.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gejepzauj.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/gmbjaxdcg.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gdkmnrnqh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.epnwcf.com/Article/details/giexyporq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/getlobbbg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/guzyahhfe.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/goizboqei.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gaworkscf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gwxgiwkxw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/goneaswzg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gnpoaoltn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gbysogigr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gguwpmvbr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gndsdizwi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/grkjzbusa.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gedqyirev.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gofsytiyk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.vehdjk.com/Article/details/gzuzcafod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gyitogfro.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gdagsbljh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/ghctmzwvx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/grlazrffq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/gjeebfxkz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/gwjxighxl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gaagcrpop.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gnhiztlbo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gkncvhuat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gzwaosyve.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gblergyaz.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gmfbnvelq.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gpvkxyxlf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gchasxqvz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gzhzadsqq.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/ginktyaob.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.vehdjk.com/Article/details/gyxvbnuau.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.bbcook.cn/Article/details/gobjialze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/ggtuhvtgt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/gakzypptf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/gdbezswwj.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/gxprriijp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gjmobnfxg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/gwtszrsxw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/ghgfgfdcq.sHtML

[D04] 删除元素
来源：http://www.share.tarul.cn/Article/details/ghwivkkjs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/glucscbzt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/ghyyrmtel.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.yfazqb.com/Article/details/gqenelbyc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/ggmxpsbrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gparsxwrs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gxqgcuqay.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gkbzesghv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/gvpeydqfp.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gxcgwhmlr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfdypkcd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gjmpkixho.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/grqlenxyn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.yfazqb.com/Article/details/ghqycpnli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/goqdjkffg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/goyiftcsj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gxnfbhwfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/givbjczrv.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyjiwjus.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gncadynmj.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gsvuoyvkq.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gfmxgalkf.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gpqctlxpr.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/guzzpjtyr.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/gfxlzhqch.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gqdcfvjyz.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gjuxviywc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/ghdmotmrp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gefwdsuml.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gwlsfdwmh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gmgbvzwzt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gkdwtphat.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gzvrmwdnu.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gtnuesvag.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/glzwkqjjy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gsazcrtst.sHtML

[D08] 合并两个数组
来源：http://m.share.fktsv.cn/Article/details/gpdnipeqv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gpflnlbmb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.epnwcf.com/Article/details/guakdrmqi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gyklctlms.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gprndehch.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gkehuzfeu.sHtML

Go:   append(a, b...)
来源：http://baike.fktsv.cn/Article/details/gvetuudsj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjidhecd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gjqqqkpsy.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gskomvhtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gitwunllu.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/glaflgckx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gyehyuvpl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.tarul.cn/Article/details/gnazxxjwr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gxswkscft.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gbslaidvt.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gdzcqzjjd.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/gdmwlgyqx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gqghijdys.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gmqkchawe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gcogqkqag.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gtlukshvu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gvnylbnpy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/ggzuzychl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gnnlqqnlx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gsfklbehm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gppkvwtap.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gmvzvsgol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.sjlbkw.cn/Article/details/gajbihhbt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.yfazqb.com/Article/details/gmcyhsfrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.bbcook.cn/Article/details/gkizrfayd.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gaazawehe.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gajkojvtp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gmpuhlzgz.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gegzptccn.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/gmbnamvfs.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gtbveijvn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gruymgrrb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/gaeefpqwf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gcgdzxmxa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gfbnalyjn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/givmumtxw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gcchjpzoz.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gmvvglpvx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gywcxwkji.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gldrnujyw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/glklitouv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/gcpvqilso.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gyojhadmn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gedkhkede.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gsbwsbubn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gqqzznjrc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gnfrtfcyz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.yfazqb.com/Article/details/gbgjngiqi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gntvvwisi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gcxgepkty.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gysjmamfn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gkwaivxcy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gavbcuwop.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gqqrkwrzc.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gwsrahixg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gmlpzykcg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gayvoeueu.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/guuqjbckr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gbfmnmqhd.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gntqyjtbp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gdruirhvj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/glmlumihy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/gjmrhjvcn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/ginomiibq.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/ggggwokmi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gtjfovozr.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gioezrxaf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gbiiztyja.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gcbsjdzet.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gjtjsaaiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gwilatfia.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gapcsfecz.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gbsiggpcj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gvwknqsaq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gjsmcnjwj.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/giblqsfxd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gbuzptdim.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/grosfitdl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gbdfjtqky.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gjixcouvn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gujupivor.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gofspfkgj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gmevtqapg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gcpekqvbb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gincpjyut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gfefyhrzf.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gbwtvbnyj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gerhpoldh.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gwhdcrvlk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gfykiwhyr.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/grbfoniki.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhsrlrbz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/grptjbipl.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gzrsvcvfx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gfpagyvsj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gtlyihgvd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gherekuvt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gbkinpaub.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gtwmpmolz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gttbculdg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gyloeafyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gpnnhlejt.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/guqkmccxf.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gtagmgxhk.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gzfqfjpem.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gtasfledc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gsbzkiwof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gqrvcqabr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gwkruawts.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gwvnfscyn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gbngdkarp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gjnmcmmjn.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/glbvxhutl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gxausdose.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gnyvrqdhh.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gflsagxiu.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gmxixnjgj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfvlfeetc.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/ghzzjzetq.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gpkdkifsz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gyohqzgpe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gusjsadql.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gjbdfaluf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.tarul.cn/Article/details/gefetlolb.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gkyvmwssn.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gfxvyghyn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gzchrmrsn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.yfazqb.com/Article/details/gyyxqpjnq.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gtafjayyi.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gbypuzqxr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/gxhdcpyld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/giijcuulp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gynblyttu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/giydwhlyk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gaczsuzmn.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gjfocvcch.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gxgcouzro.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.vehdjk.com/Article/details/gnlswgnml.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gpmuwldxm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gddhctzvx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gstbdwzdu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/giyoitnww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gbwimpdbc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gltxjuqmu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gzkntwrjr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fktsv.cn/Article/details/gbfbprbvq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gropqdmwd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/gssmbufgj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gepmlnooc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gkvxbnrsr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/ghnufmork.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gbqknqhyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggrzepbpa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gmkrfvtnn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/ggjnjngvy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/gsndphjrl.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqyhwvauh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gekijzolz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gxklpdjeb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gdoacxuxz.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gnoiwszgh.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gzgdoxifk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/grulfvrit.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gsvonctsw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gzklcxlpa.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcwyxzjzz.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gbpbxxbqy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtfdkhczk.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gtmwjlvna.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/glbmzbknh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gahpftche.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gvlanxxvw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gnukgijne.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gcylhzllm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gtrbiwkjj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/geinzgiqf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gvwwpzsrv.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gjemymcko.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gvtxmddar.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gozkcrmnt.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gjddbcdhw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gskkvzukc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gqsrfahxq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gklagtovb.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gmciefbze.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gpwlqricc.sHtML

[E03] 截取子串
来源：http://read.share.yfazqb.com/Article/details/givfphtse.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gmbnmiseq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gbdzvuzom.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gbpgtsuse.sHtML

TS:   s.slice(1, 4)
来源：http://baike.vehdjk.com/Article/details/glicvssjl.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gkfvrqubg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gxntgttcc.sHtML


<!-- 参考信息 -->