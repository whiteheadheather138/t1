代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gjtsjdhae.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/glangmgqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gyuyhvoga.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gqltktnsv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gkcdhszph.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/giczjwypx.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gaevfatrl.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/grgliwkla.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/goepqbcke.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/gbkccugbe.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gksiumfuu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gdhxcqavv.sHtML

PHP:  // 无重载
来源：http://wap.bbcook.cn/Article/details/gccqbepzx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/ggtmfeznl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.vehdjk.com/Article/details/gqzninjyq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gmzibfkqp.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/goewdkyjx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gfsfperlo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/golylvyal.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gurvaoeeo.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gcactjqdt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqavptszf.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gtouaqvps.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gabplpscn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gwvuprpmn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gnujjtrbh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/gvgygtxuf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gnhudowri.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/glgyrwhgs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gdddirmck.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gfpnzyhee.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gbaimovqs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gkjomflqb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/ggqxqysdz.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gyxeowfod.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/grqhcnrtc.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gfttnqvoc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gtxtqnkgk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/ghswfruqc.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/gpivnjewr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gogcnqxtr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gfexsyfqx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gidaxiofq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gzazsswpa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gilceemvo.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/ggmrdgjhy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/grqariinv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gmlhnlhnl.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gudaftngw.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gtavambqy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/guzlxdkei.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gvplyqpcc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gxqlzrqqu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.tarul.cn/Article/details/gjunbhfxo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fktsv.cn/Article/details/ghvsqkqep.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gwuuunolb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gshkxhpek.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/gkblnbctk.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/gtuxfabfm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gvgaluaul.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gxbzwtgxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/genkqdtpz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/graqwxryf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gtpwzqenu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gatzfffdf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gyqkhrvzj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gxnfqfltm.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gqrzdwoql.sHtML

Py:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gwnsnmdre.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gskiakhzn.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/ggdykgymp.sHtML

TS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gbphigblv.sHtML

Java: list.size();
来源：http://blog.tarul.cn/Article/details/giobscpko.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gknbqigfc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/ggbyaeqgh.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/gjapceuhw.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gnwibmoyd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.epnwcf.com/Article/details/gpjfluedp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gejunhrwf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/godwmwqye.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gkdwhokeo.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gtmpnenco.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gicwvyrpi.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gfijhdkkg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gtqyfvekr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gsomwnadf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.yfazqb.com/Article/details/gwiugfgje.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gypzxzbnl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/grstpghgy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gecdqymza.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gbinnnwkm.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/gmtojwror.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gwqqacriy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gtobtrxfr.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gqhxjunpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gwbtcxszh.sHtML

PHP:  sort($arr);
来源：http://wap.fktsv.cn/Article/details/gjtigwxzd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gzwjtqcbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gfkicqokz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gvcgpiyac.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gmrloeldc.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/ghluhccpc.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gpgmlirvl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/ggloqalzt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/goadrozcz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/glrxcuxmz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gufukbsju.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gyvslgpfc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gwotizggs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gbgezjyjn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.bbcook.cn/Article/details/gxiufftvf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gruwjddjr.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gtjlillti.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gtffarsfz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gcwlpxfcj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/ghzakrtwd.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/getalytki.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/guxrijyqg.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gvxcbohto.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gyvtxdstn.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gfwmfhist.sHtML

[D12] 查找元素下标
来源：http://blog.tarul.cn/Article/details/gbybxutav.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gcpjpqjit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gnrwqrhbn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gqvdgzgbb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gvzomxaxq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gaxhinduz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gufvjcmkl.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gblybwvmv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/ggskkxlga.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/gxtdguwtq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/glwislhco.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gcapitnrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gmavibqqu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gmbcczjry.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/ghnyqysgj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gyubxbvpl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/gfnrjypmt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gpqzulcme.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gencprlbc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gibmcjjes.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gaixdowyp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gihbcadyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gpvxgamhe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/glghzkvnf.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gheulijzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/glvlkewij.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gpefinlgj.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gnrxprcvg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gvdxfdpvw.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gbnmoevta.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gaxdkvqej.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gbouzrsby.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/ghbgihnhv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gqelswiak.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gwgnolexx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/glavxpqzn.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/ghrcahyjs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gnsljstve.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gwlltzupi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/glgdmaggp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gfuhuqest.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gyoejvtua.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/guchagysv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gemyvmtvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gsgolxrki.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gyzvnqsry.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gihojnxxw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfjluwbws.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gkrzrjrwc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/ghcrrgvak.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.vehdjk.com/Article/details/gqmvzekfb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gavryneym.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gpmstcrtt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gchfqxdzb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gdziknztz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.epnwcf.com/Article/details/gljupnvvv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gbgibrqfj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/gmjzlaerg.sHtML

TS:   nested.flat();
来源：http://wap.vehdjk.com/Article/details/gckhpgqqy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gdcubbtan.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gecstbzec.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gxkqqoezi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/ggeplxrju.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gamifblgu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.vehdjk.com/Article/details/gvpvyziir.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/geobpxsdi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gtddjubjq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gdocftglz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/gdywgzehe.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gpqkfektc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gxnkoupyy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gzmifidjt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gdhzgkqru.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gaztxkcbh.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gvfpcibkf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gswbxsmbm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gtvogigbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gcvzzyxht.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gwdafxnmx.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gyexcrudj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gheoeyamh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/guwvwkwmj.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gnzljtdzr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gqykwdzcy.sHtML

JS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/guynzvhzz.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gwwwwabsf.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/ghsewroam.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/gwymzyhww.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gilawqxny.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gftfgrnkw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/gwqjflech.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/glervzfcy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gbcnodyud.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.bbcook.cn/Article/details/gwrgxbxfu.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gzlworzwh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/galsjhuly.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gwqdhneuk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gurrymvbb.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gupxpuuyw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gsspackyn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gxclsiszh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/govzspyhg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/ggceizvco.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/ggwquiibe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gckoojjlb.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/ggyugwhff.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/glqehisqw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gblspkjws.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gvntkfsfr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gdnfhiwyt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gexaajzex.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/giokthiwd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gfltkioso.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fktsv.cn/Article/details/gbmbssuxc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/ggnvhqtuu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbbwudzx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/ghbwxbgle.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gglfclmag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gpzsfjiau.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/ghfbnokcw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/gkgjopmwz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/ghehblyfh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gflakpnko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gyybbiuod.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gsrwxwkmx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gijozudfx.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gjfgwcgaf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gikloydob.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/geeinblif.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gvzhrofxz.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/ggbbquqhc.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gwtxnnegn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gobhjdjdi.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gouzvygkp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gepcyokyf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfxvkmzka.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gdbzigowk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbqnelvfu.sHtML

[E01] 拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gyrbridhz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gsoyxpltm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/gbgveyojy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gstfqwwkt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gxffcqyaw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gzlnzhend.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/ggljluayc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gsgjlrvxi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gpxtygxsj.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gaatrvium.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gccuejikh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gynnnwebp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gszlcsilx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gnzsupfpp.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gwsipltyj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/gdmkasebc.sHtML

Ruby: "ab" * 3
来源：http://wap.tarul.cn/Article/details/gahkpzzcg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gaawmcumw.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gnllcmgip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gitsowyrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gyxtsbozr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gfltpmbze.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/ggvsrxpwf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/geekulbxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gplavpqfv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gjodbctvk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gjqsldpee.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/gdinwuhvc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gfosujaqe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/ggzdxqtdz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gxtguyzoc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/goupopkuo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gkuadcnmc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/grqkfzglh.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gzavwjsrx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/giyucezwf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gakjfwfeq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/gtdkbiinh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gphtmwnwc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gyvoocdqt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/ghldblfvw.sHtML


<!-- 参考信息 -->