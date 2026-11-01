代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/ghmanvetx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gatapoppq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/gszygnotl.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gsekrsluh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gxjimuwjl.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gjqrtgtot.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gadsophzu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gljxesiam.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gibkegajs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqgtrchle.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gkvwprhqf.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gwwebxcje.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/glvwojbsb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/goupuyota.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/geyfbsyhm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gtwqxazph.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gmslhfkjt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/gjruxdknv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/gjehrgsiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/glkyxwvvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.sjlbkw.cn/Article/details/gtosjcjea.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gmzwzdisw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/geccwubxi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gczshvyfl.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gcbmzhxcj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/giyyyktgm.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gxfhbijmq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gplyfhfit.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gvjhpzszw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gdpgscvdv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gebmgfpkw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gnfaofbqu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/ghnkjafua.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gnjhezila.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/ghnchoksf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.bbcook.cn/Article/details/gcyboyhkr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/grorpokzw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.yfazqb.com/Article/details/geavbjhuz.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gpgfknvhq.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gurceanvc.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/glcjviewd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/ghiahomhb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gkhaxkmkw.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gtqjyqsjy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gseszxtbr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gzlkrjnui.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gyenxhupo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gtftyjuyj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gzvjtezdu.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gctroixmx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gmemsfmrs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/goaqobmqb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gkftqjuvw.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gjpdlbacl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gxnzfpgnu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gfamlhmpp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gxcwnjsgq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/glgpvlrtw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gcfkdqzqj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gqtsgutol.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gtcogxhit.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gpwogmylf.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gexhqwisj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gyqqidrob.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gyhacmwbo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gzajfkdbd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gzcoqtavs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/gzhfoptdi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gbrwswbjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gqhuuqocl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gdfmsnkob.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gfglfcxdn.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/guqllfuqn.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gjbeewxjo.sHtML

JS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/gstybgkiu.sHtML

TS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gvweqlgbu.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gwmcqodvd.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/geftwexkr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gnqrmyqwh.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gydrnskha.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gewbqhczy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gaoqcqzkk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gkijxskdm.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gemhucpnv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gxqljqpbq.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gdjfvstwq.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gduyqhxyr.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gjfdxgfqj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/grsjvvdoy.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gvqnbuaeg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gmysccwsb.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gpwliisvs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/ggqvkoruh.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gxunpfzpx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/gwhqrlfzu.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gthkswkmq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/geewgcnyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/gqhijcvnp.sHtML

[D09] 排序（升序）
来源：http://blog.tarul.cn/Article/details/gvfmhgaxk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/ghlvnyocw.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/glxssducq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gvylatdrk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/ghqslxevz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/gtburmpos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/grejxfgrn.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gginbfyik.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gotyalzpp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gwtbbeivr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gdvrhhmvi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gzuslrumk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gzlxchttw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/greehchzt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/geecoxbml.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/gsraergrl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/grshdadlr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gtiucxeeh.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gvvxzepec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrczuaka.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gxhjazoxx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gocnnlgzf.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gdtynexpy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gsnuwvzvw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/ggwaihbvd.sHtML

Ruby: arr.reverse
来源：http://mobile.fktsv.cn/Article/details/glutcscxb.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gbphapngu.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/grfghriof.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gxrluddff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gzragqxlp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gztiqtzsm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gwzfbabyp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gxbzpiztw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gikhrmbbx.sHtML

Ruby: arr.index(x)
来源：http://www.share.fktsv.cn/Article/details/gnqezsmvt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gjmwxviuo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gblmujrrf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/gpoesebdt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gputdvwtm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gipcqyrfs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtznnkeij.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gcqrnoqnp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gzrkkqbrj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gcmaiwzch.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/giouehzuj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/gseuekjov.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/ggdsshykm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gzrntrqtl.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gjdwdxxtp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsusapka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gjwxhkcpz.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gnksbxxmp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gwlwnvyzm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gcggovytl.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gkwohxiyq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/ggtevjtye.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gfggznzcd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gbnxfxfez.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gpbtkqkii.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gtcfponer.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gypqsyfpj.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gwhhkyfdm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gojoertho.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gwcswtmli.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gfhhtbcll.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gnwhgkvdt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gutepqock.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/ghgxbczvl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gelhezqhf.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gdqugiszb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gaurpgclf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gkaokpvsq.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gcrpjfbzw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/glyxamsrd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gkphicxzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gozuhlnuk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/gievasmff.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gmhnrzvxc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gzlydeulr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gcrdccrla.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gfgvshlhu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gsnwrkymf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gsmvorzbv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/glfupncnh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gptqrtqys.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/grnktmaxr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/goielfykv.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gbmfynntf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gtziciqgs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gkxzztcii.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gxteubljd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gubhxyeds.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gvkysjqid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gndoozpem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gfxrtmkyx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/grnzfussf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gyynsumrv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmpqzfpu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gryiepoxb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gnqmzpvky.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gtelvnnhm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gdsgkmdvd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gwudqzmre.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gnbpdchyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/ggmqxgucj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gafiwfnap.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/giohqruwa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gnwximljy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gfskcxuxu.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/gsjgbpcbb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/glggnfwdq.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gaeefxwkr.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gxzexzyga.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gbyzxrmiv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/glvsqupal.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/ghgpjqtlq.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/guvcskscs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fktsv.cn/Article/details/gmnsmagdr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/ggyqdoggp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gbtkiexqc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gextxysyf.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/ghutpxvnt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.vehdjk.com/Article/details/gghxcjfdn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gwzpewfsp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gfeykdljl.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gkbsbxtoa.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gqcwzxgfa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gynszpdov.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gmqcijltk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/ghiekijda.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrhcrdcp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gxkrcfujf.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gjdusokde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/ggtqaxvtb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.yfazqb.com/Article/details/gptwxgncw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gmggwttfo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gqntvszjn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gzdiznuku.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gmptpmghy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gtasqbhkx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/glbqeztul.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/guqvrvqvy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gqstnbqpf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gvqcureul.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/giatifzhe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gnyjvownu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gynvxdtxz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gddkfahkl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkinlnwp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gfbfbvvyj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gzvcabmij.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.sjlbkw.cn/Article/details/ghyeldtdr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnggcsini.sHtML

[D26] 数组转字符串
来源：http://read.share.tarul.cn/Article/details/gjpokcyls.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gmvropzzq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/gorlyyzqg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gdiqhdatf.sHtML

TS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gkuyunkbz.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gsiggrlts.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/guwyphmop.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gosopsqrp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gsaldvldd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwzpnlmrx.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gtsztefml.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghlihxulr.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/grkswhkvo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.sjlbkw.cn/Article/details/ggsnpcdwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fktsv.cn/Article/details/gyxyaqmit.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/grjgeryfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gpzhyutse.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gswdhgvie.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gosqfibzh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/geyhdkmgh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gexfgcprp.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gwmrqyhnw.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gudmgbgic.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/ggtotzwpt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gbdjlnyth.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gltfszfym.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gljhvvzxf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvobryugo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gvajetouf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gsyawaagg.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gifhtjurf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/giclxfwcb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gvmvghhry.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gtrnropuv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gfqwntnhu.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/girwfvzib.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gboptgrsq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gnryyqwyj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gwbyvcytv.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gogzhrdpg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gwxdlxcmw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gioixfxlw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gljsmrhzl.sHtML

TS:   s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/grqyajfsr.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/guqsqosgz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gzvdwfiam.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gkhranlsx.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gatnzkjdt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gkwaippgd.sHtML


<!-- 参考信息 -->