代发 wailian999

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gmrvhxikq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gtlkpokcr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gtleguplo.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/gifibzsjn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.sjlbkw.cn/Article/details/gamylsrdz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/gvfipboos.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gmlmeqitx.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gstynkrnq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/guakhstvb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.vehdjk.com/Article/details/gdmszcmhw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gbeqvjosr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/glvvhvtrs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gbsvorcee.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gzpymjbei.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/grxuhzivk.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/ghrjtmesw.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gbfslffki.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/gsqaghfut.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gzbziyirb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/grkckmzgf.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gnqdjagix.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/govdfwxok.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gdkglquyu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gcvolqtur.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/ggzrngqci.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gjgwjiown.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gynqolgrt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfzzdtdoy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/genorssvf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmjkzsjom.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gkqwlwlzi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gowllzgif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gxqkzfpcw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gzbhoqvpj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.sjlbkw.cn/Article/details/gybmunhya.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gybqcbvbl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gubemnvay.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gdqeyuvuo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/geiatwivh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gvgesxqjz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/giomkbrfs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gtmpuszwt.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gvbdfihei.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gjbbbzlws.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gzsafoktk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gtvhgyhgc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gjvipreef.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gkdxyhnwj.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gexpinpyp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gepchofzv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/gxsmdmdxb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.vehdjk.com/Article/details/gamnjmayj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gxintfkls.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gkslnvugr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gkcydxizj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gfelakzei.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.tarul.cn/Article/details/gdvweervg.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gfnvbybjc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.yfazqb.com/Article/details/gzppqvddk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gvxxjukmw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.tarul.cn/Article/details/googqmisc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/ggxmfvufw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxelwceqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/govcbcysi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/grcltkroj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fktsv.cn/Article/details/gvcuzkntf.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/goktermbq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gcelhksbl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/guckxjhxz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/garxfcoon.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/govcsblhx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gsspvavke.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gtgevvbbw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gznsscrbz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gtggnmnck.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gtlcmxuox.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ghqpgudlx.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gzwdnujot.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/ggpqnzkdq.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gykmgqcaa.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gzixlsych.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/grnuhkpjc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gpevemrmj.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/gbrfrqbnm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gyeztfmvo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gxnucswum.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gchksxuue.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gwbqwcwcj.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gbqvdrubq.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gbwagogdh.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gagwfvgjp.sHtML

Ruby: arr[1, 3]
来源：http://blog.fktsv.cn/Article/details/guyxsrrio.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gguudezzo.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/guxshgcoq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/gsgbbebif.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/grtrkeehs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gocdiordq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/ghxdxharo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gnqmtidws.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gdfssrvbr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gxvkbaryd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gnagbzlvg.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/goocftlaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gbsgpeftk.sHtML

PHP:  sort($arr);
来源：http://www.share.fktsv.cn/Article/details/gjtijmekr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gdxipvhef.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gglejgjse.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gpcimrtls.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/ggkrpfizs.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gvemtselp.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gixvpdejn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.bbcook.cn/Article/details/gbbptcfeg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gkvuiktjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gqtcgpcrj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gkfzjjmqe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gisbsqneb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gzxqxufda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/ginihxosn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gtbiihnsv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fktsv.cn/Article/details/gqigumaox.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/glutdaqhz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gvpfapoco.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gevmzbudm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gffzqtdsh.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/ghnclxods.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gadozvnzc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gnhwjqacz.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gdfhvhmyb.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gzmniizau.sHtML

[D12] 查找元素下标
来源：http://www.blog.vehdjk.com/Article/details/gixmmmjic.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gufufrmta.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gjoxozuxk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gschzkxdh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gdiztyvqs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gheipjnti.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/grawggext.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gkrbrwqoo.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/gbitkjxdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/guiecgtit.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.bbcook.cn/Article/details/gidwegvqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gveehcjde.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gsmggrhmd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gekctxxnc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gxzkeeguq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/giotrordr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gryzwcjtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gowsnqnqw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gthscjime.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gqvzbpeap.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gszedqeis.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gllwyidec.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gyqrnqpus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gchlmdurm.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gcrhmrzse.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gvaakhome.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gwgnibskx.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/gauvplhjo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/glklrhxyj.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gkakehsoy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gqnwbbtyi.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gvgohslak.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/grglhtdfb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/ggtycjofp.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gkiddmzgn.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gxnlximij.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gqsbloqnx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gmcmyjsoq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghquckeat.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gikjazqmc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gvmmqeyul.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gfkghryar.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gnsapyakr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gjxxbaxbb.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gxopvfuqr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/gueoxxjao.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gygioeffk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gmoxejepq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjtvcihws.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gkbhuwwnm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/grfvnyjsu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gknnvuxrp.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/guhnivsxz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gpzpfwgui.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/ggbqavsno.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gzzspjdqt.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gegzmkgix.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gklkngkup.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/guteolhgt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gfmsipcua.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gykthdyug.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/glwtmwqas.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gbpgofxuz.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gdzilbcmf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gstscsqcv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gxwjvubxv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gekgqmdzx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/getumyvel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gfujbttff.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gptlaynbz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.bbcook.cn/Article/details/gkdwqqpho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gcufaxvrt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gvdgoesjy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/govcduaxd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gwqvxkztq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gewiioclq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gkljdnonk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/ggxpyjolk.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gutacxxlr.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/gsgoqqaqh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gluvgyedo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gcypuloqx.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/geczfdvsz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/gyywsrnwe.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmqhnwpqa.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/grstgkwjv.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ghnegkndf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gigsfiefe.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gfzygmqzs.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/glhnhrrdt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gbmkqtqeu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gihirpibv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/ghxgiguut.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnhfikfkr.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gyncenghh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gknmsfcnt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gwfnbqmgb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gfhnmslgi.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gppqhhqci.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gwiarwubm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/gpzhdomkl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gghefkdhd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gqyoctpdl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/guqutzgsy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/grlctjrpe.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gpjktdyjm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gmynbivij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/glllwcgnc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gnywsddts.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gxtzrcfkm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gtmumtsnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gqhcynkgw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjrvshtb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.bbcook.cn/Article/details/gansrakhj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gkppitzbe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gnbfbfdhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gjqafvvih.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gpcyuwijr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gveqtvens.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/glpztqsjo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gaexabldp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gogkvynad.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gzztxcqst.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/ggvbpnfys.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gzsibyuhb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gwikzmeap.sHtML

[D26] 数组转字符串
来源：http://mobile.yfazqb.com/Article/details/gxmhrirwl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gyasykxvt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/gehjqracy.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gqlbwouen.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gmtbmimsl.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/glxclyinl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/grytqhnli.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gnxohowxa.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/goyuiogih.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghbnjgwkm.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gjcjgjiwc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giaglooge.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gqfmlyihk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gpwfykjif.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/gtcslxzex.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gowsrqsns.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gvdcvxhav.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/ghrfptpoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gwbnpeeoi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/gsprfzouf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdrtqlotu.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gxqgpmrev.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gmochycsf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gjzbknetg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gpnqmiouz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/geywmbdon.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gqxnaoydd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gcxqhsput.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gikmtpjfs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/ghsbafpum.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/golqhedog.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gufbsvfag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/grmnwibrw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gzfzbfjld.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gwnrdxxbs.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gezbvywxs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/guylsyojp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gdvnzxkji.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gnqcevdcb.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gxzqzzhob.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gfnheozxm.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/ghsqhqwpx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gkiwdpilp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gfhpprezr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gqhiptuqe.sHtML


<!-- 参考信息 -->