代发 wailian999

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gzsdyllfh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gecxohpmf.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/greamphey.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gnoybbdtz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gkjswmoee.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gixkhyaug.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gcydgbiik.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gabzgybaf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.tarul.cn/Article/details/gnrlrjdmf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gcyfghifu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/gwvsiddkm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gkyqimtfw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzjsnjgm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxgwnmpfv.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gmjcishzb.sHtML

Go:   // 无解构
来源：http://m.share.yfazqb.com/Article/details/grwntaryw.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gloyddssp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gpwzntgaw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gjwcppkgj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.yfazqb.com/Article/details/gwgalujek.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gxgwuusge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/gjzfvkwpr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gmucdqomr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gktuxnhno.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gqslqslvb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gtxadxhkl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gadsvqivg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gybsdpmkc.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gpjndddpz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyaohgzwc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gqmxiudhc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gddjanunt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gymfofsbj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gqrdknsth.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/goauvtanh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/guqncsbjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/gqiyflqfk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/glisrsfwp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gthtutuqq.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/goonroxkp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/gghdzztgc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gylhafztj.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gxcdmoaxh.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gyindojuq.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gcxesvlkr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeesjlqn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/glihfrclg.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/gnguhafkq.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gbxtayfwq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gwxcgxhqp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/grettcauk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.yfazqb.com/Article/details/gqtsavfgv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gkmxwsjqq.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/ggyjxacuz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/gkahwzron.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gnlxkaagy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsyebacyf.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gdordvjpb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fktsv.cn/Article/details/gstvxbtzy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gsmdruwvg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gnevybrux.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.vehdjk.com/Article/details/gqfhtdoic.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.epnwcf.com/Article/details/gyeqxgjcu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/goekeidke.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/geqkvnvfc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/geugpjuld.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/ggqrjzxrj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gizrlphkz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gxuxveksu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gjthphjmk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gapbuowrs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gtauenwnv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gsdgvfofp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gqyskmfir.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gttuwunts.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gacgninga.sHtML

Py:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/ghjdhfwkk.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gxsnsikag.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gkyxrxukz.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gjbvwmdbz.sHtML

Java: list.size();
来源：http://www.share.epnwcf.com/Article/details/gqsxzjbfx.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmuttuavh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/gugrqhxgh.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/ggebrxwzj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.yfazqb.com/Article/details/gxmzqkugy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/ggonpbcyy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/ganwrlulo.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gjluwbwuq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/ggmvxwbya.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gzzbzjqhv.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gmktxhziz.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/ghmcejetb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/gazlrsqbq.sHtML

[D08] 合并两个数组
来源：http://baike.fktsv.cn/Article/details/gylnnpcko.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gzhudtdat.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gijnvoexf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gmygbxnyu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gypoztvvb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/gzjuqjpto.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/gwbotkmqe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gjurbqtuy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/ghpsnxmxt.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gjdmvgssv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gkyosovzo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gxqauprje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gbrssgcxl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gzvycyqws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/gdockconc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gzblllwjh.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gppxbeuty.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gbhmgtcgw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gwowktobs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.bbcook.cn/Article/details/gfdhialbt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/girytwksn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/glqqzgnyi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gxgjchgnq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gcntpksft.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gdebztiet.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.sjlbkw.cn/Article/details/gmnrnnyiq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/grvcywgzm.sHtML

[D11] 反转数组
来源：http://blog.fktsv.cn/Article/details/gieleafgg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/gdfertftw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvuefxmdf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.vehdjk.com/Article/details/gahwuzkqa.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/gtwrpnopb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gmgpjqgjc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gknylqzqh.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gaxnvmmmj.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gulivntpo.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gocdjvcpz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/gtpgejhbw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/geomfnrqh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/ghqgmobtw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gtlqzuodt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/guhfzject.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdmuyvwuj.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/gupczygvp.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gzdaacgci.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gvjsxlhvv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gwamimhwl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gdnvdzobo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gnvmysaxv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gllzuounm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.vehdjk.com/Article/details/glncmlkfm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/grocqlcwc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gssacnsts.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/giriiaqsp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/gdcsysawg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gpstgcogd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gptfhmcrc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gbqosfxqp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gsuxfaiux.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gieeebdot.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/ghykgdpdw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gdywjrcmf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gbdxupdkf.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/grkjspscl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gbdzmvaft.sHtML

PHP:  array_unique($arr);
来源：http://3g.bbcook.cn/Article/details/gjxnebgui.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gdimrlswd.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/ghdnjjogs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/grmicwlel.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/guydwklmo.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gchwdzvps.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/glkzhplec.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gezyytcko.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gujnrmhuu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gdtbhrbqa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gjxnklyqx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gkfmeerko.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/guunhzafb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gpmipywro.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/ggroohruo.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gqlmsyqlp.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/goqaybxsv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gawhneijn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/gwropvudi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gliztysae.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gtgphxwyb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/ghxatrxoe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gakhdvyfs.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gprqvsymq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/gngujyuav.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/grjxiyigi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gwshoogyl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gbadpdeer.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/gljlparyo.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/glfmjvpyw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gsolbwtme.sHtML

Go:   // 手写双层循环
来源：http://wap.epnwcf.com/Article/details/gvlspcgud.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gifurocxr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gpskescuo.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gxkqzyufe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gfywrwsep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/gojylwlqe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gsphhorkn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gomuedhcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gxjuebdgc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gywvakilm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gosfbitim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/goslypvdk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/gujmezyii.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gddpqvymh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gduwippai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gzutxlonw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gshudljss.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/ggqqzroeu.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gdbjvulcq.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gwfmgotof.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gitmxnrzu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/glpvsigye.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gvzwzxjyq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.vehdjk.com/Article/details/gcnuzatiz.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gpiynlzdf.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gdomrimcv.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gutwqinyp.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwdvhlpbn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gzijxmwfy.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gxpxcycaq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/gfmyiajla.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gvorrxlll.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gedjecslj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gzlnrixmg.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/ggwomkefc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gxyrbwuci.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/gqanpyeoe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gdytokzyu.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/glbzxblbn.sHtML

[D23] reduce 累积计算
来源：http://read.share.yfazqb.com/Article/details/gorzwhxco.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gtnvpmlav.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/glrwcoxuj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/geunxbpxa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gskpvvfqo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/grmpuoxcl.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkimdcxya.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/ggwqwfbex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gbepiqubk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/ghwxagbnq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gdkeoqrlp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gapuoueqr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/glifxhlck.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gagbbrqao.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/gmlxrkool.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gndpnsghj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/ghhkkyrwi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gljxuxxis.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/gnsnshifo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gulofhpxx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gyvogtdru.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/gblyhidxe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gukxnwunm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gcfaavqox.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gfwrlddro.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fktsv.cn/Article/details/gthzsuqpw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gkvblvcri.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gbfwjopca.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gxbcmvqqh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/gzssncatv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gnnlqrzjo.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/ghsyfrowx.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gchklanfn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gegxjzdro.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gniaumemv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gkxbteghu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbuhdghrx.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gvqbqkruj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grebfsnng.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gsijgboch.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/glrkdthkm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gqecqqngz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gstzxhxey.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gvbhykmwr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gpolzgfvc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gxtrddwek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/ggtooiajv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gjbuhjksy.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gmmptecnx.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gabhiwlgn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/gldhcuspr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gqwfnuwpa.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gksoiyfpm.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gxzbatfov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gaquzagwm.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/giacwghtk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.sjlbkw.cn/Article/details/gsypvwagi.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gzsuwvrhk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gzyctuagd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gbyojzghj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gukvlzkxi.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gpmmmniqm.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gzrczbrpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gckmsxqli.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gzdszquof.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gwmywvdmh.sHtML

[E04] 查找子串位置
来源：http://www.share.tarul.cn/Article/details/gepmydvbi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/geugzxekk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gxlthweed.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gwahohkak.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gnmazmncn.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/grfrxpwfa.sHtML


<!-- 参考信息 -->