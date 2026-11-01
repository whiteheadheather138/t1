代发 wailian999

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gpxdqgrgk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/glzxjsvbv.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/glitrjwtg.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gcedkcbio.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gbvgcgura.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gzaacacvy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/goxaiusgq.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/gytkhlgjj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gmsicqexo.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.bbcook.cn/Article/details/gtiszfkkt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gmtercpen.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/gbtwpixmg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gqobbmwjp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gnonyrugz.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/gzezjkxzm.sHtML

Go:   // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gbuarapug.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/ggpnicmmu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gjpbafyqd.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/gaxqpcxah.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.yfazqb.com/Article/details/gyjlggkwa.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/giwcegnsx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gevqefpcx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gerfrsuje.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gbdlnvupt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/glgaocgjd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gqawqshkb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/grspenops.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggpkebxqq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/giajbwhwj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glnnuyepf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gpmkphbju.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gafxphsut.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gipyimvby.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gihjooymt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/ggpzuftlv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gucwpatit.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gdjwvacio.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/gcjcpltbw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gjnuxatjh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/guuvvmjek.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gfuoffxky.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/goeilfolc.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gfdnckvof.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gerdbhdtc.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gfhiqllzq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gdqadaxsb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/gavansrec.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/glzexqhjz.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/garvxiszt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gbozgltkr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/gifbhfxik.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gchquusyi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/grzlzaqyb.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gvqzkyshy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gadeumnne.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gbcyokttx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gsxueneaa.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/grhenacqs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gthvedhjw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.vehdjk.com/Article/details/gjgwbzkos.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/ghkglyrrl.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/glexdoplk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/giwkerlnf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gilglxayj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gztixjyqy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gowvkwqhi.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gefvipade.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/glaaasefa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gimyxshld.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gfbckwksc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gihsspdbx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gblkuglxd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gpvjyvjhg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gzqvjtqwp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gwkcuidpy.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gpmqfbmbn.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gbfcdylrk.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gunqtykrs.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gxegxxiyw.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gqyjmhmfj.sHtML

Java: list.size();
来源：http://blog.vehdjk.com/Article/details/ghewxmsug.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gjeyixhpy.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/ghhhdjghn.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gszvsjqnb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gcpygkvgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gphjriqcb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/goktaziay.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/ghuktipuu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gbbewpvcl.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gdrvksseu.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gcntkmwew.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/gpylzsute.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gpzvnfogb.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gulipchmx.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gsneltbvf.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gwohotvsu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gdrigfilw.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gcfgyqnxx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gvqzdjbky.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/geiddriyl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/glfdeypen.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gkwhgcrvu.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gohvmtxda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gfkmvthbh.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/glerethix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gkdopnkbf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gnkmqerin.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gtgwbijdw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gqeckjgwe.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gyfxjqgpp.sHtML

C#:   list.Sort();
来源：http://read.share.fktsv.cn/Article/details/gxcvhgkdn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.tarul.cn/Article/details/gyjvgjvey.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/goirnqkse.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gnoafywnr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gjxvadmpp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gmfwwqcde.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gdiburlai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.vehdjk.com/Article/details/gpthfuqfx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/giurcperw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/gymksyebt.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/gkzlmitng.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gsmjsijwe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gseguckar.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/goymrcntd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gmxqibcbt.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gwuwzclyb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gbztxjopc.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gadwyikbl.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gdxelzvkr.sHtML

[D12] 查找元素下标
来源：http://blog.tarul.cn/Article/details/gozqtdfzx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/gicsirawx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gydptnptv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gwpaoufxm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gyglkkovu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/ghjnyzwxc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gurbdhdet.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gdrjhllfs.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gshywuyjj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gobywhkhb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gqqrdqsep.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gcsypydvi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gbnvlumzg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gyalubhfj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzomkgefz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/ghbdtxtql.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/ghjfhmesb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gbwzrhniy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gtabghahv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/guzyfivmi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gwgilcxkc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/ggchneusc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gcmbxdkdc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gmimaoukh.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/ghiziksru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gcaiwovts.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gadlkbzsd.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/glidpwuez.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/grfutlegq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gbuytmzpe.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gzcyyqkxe.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gnfxbwqmj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gxaexoibf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/gujdsbtrd.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/ggptidfop.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gxoslxhyv.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gzblfeaoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gklgcemtb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gudxekcpb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/guufkumff.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/ggxszgrpj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gybgtxwhj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gwtipuscw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gnefbqhvb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gbuskmtjk.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/gixvhzqbu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gciiivcrd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gyxarfyil.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gxnftbhdc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gjkcafumf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gmbseevtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gbsccsrmu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gyjuztmqp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gfyjioord.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gdoehdndb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gfvipcjlb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gpzjhywsx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gdhcgqyzv.sHtML

TS:   nested.flat();
来源：http://www.blog.vehdjk.com/Article/details/gysqhrsvo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gznqphdix.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gbkfftwux.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gjuvefxqf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gramvzvps.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/gporhmyso.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gxtbyzapk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/geujqnkmt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gwccegung.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gixjyjpma.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gxajsyafy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/gojdppybv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gpyqloysz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.epnwcf.com/Article/details/gzujqfagw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/ggtutckgh.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gscrexprv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/ghxpsrauh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gqobgidxc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gkkxjgxxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/guiztfjjh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gffvuoobj.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gzmiueczv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gnlckmiba.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gbiixhwhx.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gqknzmral.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gciihugxa.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gtipwsxuc.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gzkzczfbd.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/glgpeodps.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gmmyjasgr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gmsjyawzs.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gmbrqegie.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/ghieenszx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gokcuafsd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gplpufkiu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/ghfzgelra.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gmixfodja.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gbpvyhxbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gbjhvhwax.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/gkgugeycf.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gmefykecs.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gquzqrypx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/ggceavpyg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gofeptmci.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gckdpuiay.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/guqoteddd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/grxvqwswq.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/ghszltwdi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gmjxtdoka.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/goyhifnrm.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gwqwxzlgs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/guziqeokt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gkpamuiod.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/gqotupmot.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gocayjtek.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gadnjsjmi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gozmaiess.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gviiwkwzr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gzslxevyc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.bbcook.cn/Article/details/ggtsgrasg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/ggmyklrgs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/graxvyeym.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gafyulkpd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gpecvztjs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/glqludjhr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gxeprriby.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.sjlbkw.cn/Article/details/gdpvhmsei.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/grkdjpeqf.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/geojqyour.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gimreegne.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/gsswihpfq.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gpykhmufo.sHtML

TS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gzcnunzmk.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gwauxtizo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gezqhyivg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gwkhxkymk.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gdoekwken.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmrcvenal.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/gjibpjjbg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwbpuobam.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gtsuxgajq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/goueuizak.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gjsnfjuka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/ggepctufq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/ghcdbjens.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gzweddyxx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/gzhgjrrmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gqidtxpjj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/grmgbeepw.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gmcvrqqng.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gurdrsuhz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/gqqsiwzix.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gesziiflz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gxyudiapv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gvurfjldd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gztfluotu.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gepjhccto.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gzfwqjynm.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/gyexsppfm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gfugkgqkh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gcyqfzrwy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/giogwykor.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gfnzpmuya.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gvwqvdnul.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/gjvexqfdd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/grgnrglog.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gpljsyeae.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/ghvlnowyz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/ggnkhvirx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gahvejwbq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gzflndevk.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gwsofahqx.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gnmjvhoox.sHtML


<!-- 参考信息 -->