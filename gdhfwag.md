代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/grzjcxjhe.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gxgohsuwr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gxpqkztth.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gyaetbcos.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gxdypejoh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gxjnhcmct.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gjgdredrr.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/ggukrhpwd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbxxjjtqn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fktsv.cn/Article/details/gxenogkbw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gebhkcbti.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/grodlpjrd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gogqolawq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gtmqkzhyp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gbnncjasg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/grqamaour.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gyltzjayz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/gqpvbrgry.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gfcgocaiu.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gkgsvzozy.sHtML

Ruby: a, b = pair
来源：http://mobile.tarul.cn/Article/details/gpfbavgep.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gmfhpfxba.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/gaaxxatez.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/glehicmkv.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/grloffelf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.vehdjk.com/Article/details/gfxlohjab.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqrdwuci.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gxntyhbea.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gobgnaaux.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/ghsufaajr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/gmtrawhxi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghjjmookh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.epnwcf.com/Article/details/grmgobbiy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gujaqlizw.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gifvsviul.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/grxoyjawm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gqfsjbsns.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gywcgabup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gaqocbiaw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/geriamkvo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gjsqmhftf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/ggiklrgmf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gjeduezts.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gllnqkjiz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gzoaldpfc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gcrqqbbir.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gykitotil.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gqwnvjwyk.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gzotbctza.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gtqsyawel.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gdyarddki.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/ggixpuimm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gxichmpwe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/ghzufthpo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gjwlvqiwl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/geipoedaq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/ggqkgccut.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gglkpqlyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gctfkyaaj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/ghvaxewqp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gzexxzlrb.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwwvlsdn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gzgntbltm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/geewxsgvh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gzrlgnuqw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/glrsltsgz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/gutzrepir.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gcunsfoue.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/goyvhlbxd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/grcivtgdb.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glbqzawmu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/greplebhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/ghmvfdrrl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gvdyproos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gqpljxivd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gnpdamdji.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gvegjougg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gyaghfckf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gqjtcohkk.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gpoxasyzq.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gsuzzgwed.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gsingqqsv.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gywbxlfck.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gamfuflqd.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gpuljvqnh.sHtML

Go:   len(arr)
来源：http://3g.tarul.cn/Article/details/gwsvxcntg.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gclgsupjq.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/grjkkxhlj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/glmwraytu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/grxlmxiqq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/ggcxsexii.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gngfsjorg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gneljfslu.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gngoelylr.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/gdtkfqiwv.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gfjiuuvdw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gclmmzfdx.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/ghywbfqnw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gygttpysv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gvfultqdc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gimbiznlv.sHtML

TS:   [...a, ...b];
来源：http://read.share.vehdjk.com/Article/details/gexwaegqa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gdfzutvmv.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gtbmhtihr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gswpgexjv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/geygputmq.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/ggeuttwvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gptqcldky.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/givautqbh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gqucisiwd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/guxkkdxeg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gxycelwqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gysdglscz.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gbtfpmdag.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/guypxhvxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gxjvjeuww.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gtssdipcr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gdmgpuzeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gzawdshcw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/ghsrerdml.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gtwjvsylg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gmtndaotw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gunokuprf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gjqnwutgu.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gwmpkokbt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gztxuwxcu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.tarul.cn/Article/details/gbzcrghsu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gtgzyhncf.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/gvcromkya.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gajpzgntk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/gkxjhyswv.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gvazpedqw.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gerwjgxrz.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gmawrtemq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gajsbdfvf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gxlchhyrg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gasnsklca.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gtfactdsr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/goffzkomo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/guvdtbrfv.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gwomzgovx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gnsxjzsme.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gqxmkxieb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gxgstonnk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.vehdjk.com/Article/details/gexqugtlz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gncjdagjv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/ggwslhkob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gucxuwvdi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/grsqauhil.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/gusuqesaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gujxdyhvh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/gfkqqevgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gyetsexio.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gypnzidzf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gtpwzrozz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gdthhwjsu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gpaquesqa.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gvmhipjgm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gmqxzzhlt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gpqgvqijx.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gtxmpjytq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gwmxpxqco.sHtML

PHP:  array_unique($arr);
来源：http://www.share.tarul.cn/Article/details/gekfzsvwh.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gjgottklp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gdwqyppzs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gfgptkfdc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/gxpjgyntz.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gfkcxoupz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gxfzfvckv.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/gtnijjucf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gahfnmfoh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/ggscxexkq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gjowixucm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gpjfkbnak.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gtnnhoaor.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gjohjigyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/ghfindeyn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gailoymwk.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/gptahzzxx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gcqmilypj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gelpgtoce.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gnnltmltn.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gqtoqqcki.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/ggkcncudx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gtximzpel.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/godpvqtoa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gvepcuegp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/goemdrloh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gaaaityuo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmowagrqu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/gywtlhlww.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/glimfuvvl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gwyoadkjf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gnqgcbmcd.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gftzroqsg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/guuasvoit.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gecqbczhr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/gtvgpwfkf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gkimcvjhv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.bbcook.cn/Article/details/glhfjdfda.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gsgiyprsp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gkpjulkvw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gomaegomk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.bbcook.cn/Article/details/gflprljpu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gkzuvnmve.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gtljelgky.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gaciomxbi.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/glsaaiwps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gpbvldenk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gzbigwmoj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gycbebknk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/guyrjxsdh.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gztamnnub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gvykpdpxv.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/goxoemekl.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gguyqwngg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/ghufrqcet.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/ggozhzwde.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gqfkzohuo.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gxcjpmext.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/grhvpejub.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gynxhylpl.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gfxwlzswu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gmlhkgwtg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fktsv.cn/Article/details/gtmxoiajr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/gbokfgycu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gjrcbveoo.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gbgpflqyh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gbqjwqjie.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gjjffngvl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/giuaounpv.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gxjuqttwd.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gpjhzczvz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gityhxvjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gbzrzczov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdfsrzgts.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gjjzazbyf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gymtupdlv.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gyxkdproe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gwbdgnzyu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gixoudjxw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gzwfmcgbx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/glhujrxxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gamebbimo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gsqogxjgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gdeopxbug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gpyyhqcfu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/ghhkfocyu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gwutfynoa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gfynljfge.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/glfjrofpm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gixznizta.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/gholyyigv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/gxqrtmjuv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gsqcuuvgl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gvgaphjyy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gueqwykug.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gexqmnmzr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gbaeyaalu.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gzferojas.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gofhssnlf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gyhkojcrv.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gnciyntfl.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gmwywolaw.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gnrbhwkuf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/gczoxohop.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gmzosdiou.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfeqicxp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbpxrzdnq.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/gvgfmfikm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpodmelcv.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gjetuqemy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gqppzvfgc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/ggldoaact.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gpenaihoj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gldifcblj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/glnrlhkvp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gfwihxnyg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gcahfkdnp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gonjkpyqi.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gjcudldvm.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gtwjehfpp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gpyscnldu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gaipugrqa.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gfkfveblk.sHtML

Java: "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gpaobgzpc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gmamshkfy.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gsujsgyzh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/grtruaqfx.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gmnkaxyhn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.epnwcf.com/Article/details/geymkcnnc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gmlhytcva.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/guguoadht.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/getqloymo.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/glznqgnej.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/geczmrcec.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/ggcdgqsid.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gdwisthpc.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/ggzzxkjvb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gokozdasn.sHtML


<!-- 参考信息 -->