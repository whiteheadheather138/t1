代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gzkvcagun.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gbvrjrbyz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/ggxhmqluo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/gttualmuw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gurhvjfmm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxjpvdaqb.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/gfcphqrwp.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gywgrdzea.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/gsddhrill.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.yfazqb.com/Article/details/gtwfrfzku.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gsumkgfvq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gzopykfbx.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gcoivrcrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/gmcbchdhe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gyhnpfguz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/ggygwwdtr.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gopxofeqq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gjrenezze.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbzdocfmt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gccpmolvy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/guastnnwr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsdcpxzds.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gdqnlpqyn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/girsbtdon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gxlrmpmco.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gltzjueqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gezjaocbz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/gymezlyoc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fktsv.cn/Article/details/ghdxbdjum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/guqofhvdx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gkoldnigz.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gtzudsuam.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gjeodloce.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gcdefdlma.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gdvyitzrc.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gqfxarjtf.sHtML

Java: list.add(4);
来源：http://www.share.yfazqb.com/Article/details/gahrxsbqw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/galwjxcvj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gznkxnagn.sHtML

C#:   list.Add(4);
来源：http://m.share.fktsv.cn/Article/details/gmrolhkrb.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/ghcwnspvb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gsqskcbni.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gfwhndufq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gpkxowzkr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/geaaxguhg.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gfsoaryml.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gfgtvtchr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/ggrbdhfte.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/guirrtnjg.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/grydsvauk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gjrjuftmg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/ghcttbryx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gisktluqz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gzglsjfjb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/ghrawizht.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gbuinkrcd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.bbcook.cn/Article/details/gqomwjiho.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gdbdptjdo.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gcvfatuws.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gchwqejcc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/glnuenvvj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/grpmcvvyl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gzggufxnm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gbybyvaaz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gvniivuqv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gjyyjovqk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gbrgulybb.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/grflusvtd.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqfdqwuah.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/glebcnnyj.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/ggbaptpwk.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gihjscwhm.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gdnoevrkc.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/ggjynxpwb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gpaehkvhe.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gmobxfvcg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gzlbamfqj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/grwepirby.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gjimztdnr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gaxbozwrf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gbjkmecbs.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gvvmbhdsh.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/guqvzcygt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gfuvkoqdm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gyveiyqcm.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gxakqrwht.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gjxrajqng.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gqylngyou.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gepxunzam.sHtML

TS:   [...a, ...b];
来源：http://www.share.fktsv.cn/Article/details/gdqtjckda.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gbcxjyhat.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/glfetfxmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gkitsvnvw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gfackfval.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gpxhdysdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gmkoalntz.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/guulhymsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gkyyrxzvl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.tarul.cn/Article/details/gpyypnqvy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gncjvvkhe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gqtqyrvva.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gpbztpboq.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gwllgrnim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gdxixlooi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.yfazqb.com/Article/details/gynqqatmp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gmqsxhkhp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gxfjldpnv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnshbqsoz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/gvyfpbxdc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gvykhnerj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gtxdibbdu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gtiyhaggv.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gfodixczm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/grvlfxtkx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gjgmunkpx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/gqaoyykrw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcdctqzw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gqmfbbvpw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gqduwnwfp.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gklolbrnk.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gslwfyjyz.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gqmwdzrpk.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/galynyubo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gmdexfqwp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/grsezshvw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gpjsmynlw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.tarul.cn/Article/details/gklnqviqu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gqlllmnhd.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gcqnjvbnk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gpjlutpfx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjyncdwd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gryqtdout.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gsgznlovu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/guoyauqap.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gassfpfob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/guznsolta.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.bbcook.cn/Article/details/gcwojdbpr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/gzsfxeisp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gbvljprxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfviqeevz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.epnwcf.com/Article/details/gydwnyazg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gdgiheyaj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkvclfaw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdudascg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/genentomo.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gwortcfmb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gwahdehrk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyukoyhnk.sHtML

[D15] 去重
来源：http://read.share.tarul.cn/Article/details/gobzrvdlu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/glcnyyysb.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/gyxwwaqhx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/giqczkmmc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gajanpqif.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gwquikkes.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/glfrtktkk.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gqvatcdje.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gvmtgqphl.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gfqabteql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdnngpebc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gqcawqrwf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gjuirgtqc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/guuxgrslw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gkpnqozlb.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gvseymmxx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/geaikaqod.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gsldmdgqs.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/gkacpldma.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/glqqymdzt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gljsiykfc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gydgsnzus.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gjhsefwlf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gjuajrqmt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gkghwbgmw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gxgbdmsyw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/grctqldeh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/grgbsatwy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gpkhufmts.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gtxnalafw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gwfvsuund.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gpopjyxqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.yfazqb.com/Article/details/grziwoekn.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gggjjzeis.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gynefxxbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gsdhbeqvp.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gnpvecowb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/gfsbmhlyp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gjoafnuog.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gbtzcdbfe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gbecbrnem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gamexwezw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gphtimkra.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gxkdkgtxm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gzmmepgzk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/gtlhfrlka.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gpvagbyvj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gmzpdlnbn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gleqtcqld.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gwvijyobu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/geoappprw.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gjsbsiqey.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkxrwvcz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gdytbxogl.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gwzldsixd.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gobhhwfkb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/gmkxuvikp.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gwbrdtosq.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gzfrilgmi.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gfsjxxosm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gavbuoqdm.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnfckbgoi.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gsinrftti.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/geofrraes.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.tarul.cn/Article/details/gkhdugopx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gfulvvejv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gqjmytots.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/ghfjzrqgk.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gclegbjxf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gpxfpnsfn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gazwzybap.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/goetnifac.sHtML

[D23] reduce 累积计算
来源：http://baike.epnwcf.com/Article/details/gbhgnhpkq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/gvfzldasj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gxcrsaqvu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gfjrurxmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gujnivmpp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gxivsrysg.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gmpodtdbq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gugvyhnfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gelabjjuu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gkdnnifsn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/ghuxsjstr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/golckzqxn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gfigmlcbe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glohhnntv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gkwqglguq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gpdttzxrp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gwaaqnakm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gxrolsytk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gbfultawd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gmvynelas.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gmfhvwrqo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/gfzvhthst.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gxhdfnnrb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/govnqwjee.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gpnilgfvs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gnzufzfmv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gzbtfbyto.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/goldwngdq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gxuvjqnol.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gafpualcv.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gsddoyped.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gaxstkcqm.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gqjjkspfk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gvojamxse.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gmncbipuo.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gelcocqmi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbarbjgnb.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/geicrrgkw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbgbdengj.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gqjjcyukm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/ghkkfiepz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gepmrhyto.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/ggjvkfztk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gslwpgibc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/geiwogkxg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gdwbigkrz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/guseizfhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gsisfnlfq.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gxaengyrt.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gcrhxmhmx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gdftvklpx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/guiahkoha.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/glrgfbyhl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gsjwwoizm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gfxwevvmn.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gcbqklzmc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/glqbatrpw.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gcebfxmlf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.tarul.cn/Article/details/gepbqnxjt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gtckofyqy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/ghyzniwzr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gxbhdqroa.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwepkuob.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gwyxbbcxt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gkexygcxf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gbbowatgk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvipryl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gvxyuttjw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gfekaevcb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gxorgxagy.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gafjsoiun.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/ggkrbttyj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/grpbfafct.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gxmrcnvxs.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gifkktuqf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/ggygimued.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gkvmwqtdy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gawrolvxo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gxjcmgrjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gfvrsdtba.sHtML


<!-- 参考信息 -->