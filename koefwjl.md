代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/givokmlqi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gkvmlryeb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/grlltnxlv.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gmzrodkpq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gydilitqj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gbxkonrlp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gxovadlum.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/gjarmwbdo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/geoudgipe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/galazzhhe.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/gzumybrpn.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gtbzsqgfu.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gafzustxz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/gzvalnlre.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fktsv.cn/Article/details/gpnekjlsk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/grotngpxs.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gugfwbmtq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/gilxdynhw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gdsseupbd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.bbcook.cn/Article/details/gzwbbrxhd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gsxzvisvs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gueaektjx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gjvdpmfrz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvwxpequp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gcfsdzcmc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwgzfxkob.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gjhexcuvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gpgozynlm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gieiqpuiu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gxlgrujxu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/ghxtemsym.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/gymcdszwc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gizrxeuvt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/getmklryh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gaysmeupe.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gjdppexmh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gqoclhare.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gippvlepu.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/ggriyllct.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/guohrzmtq.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/glhesmcft.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gjwxslutt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gckygbrba.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gaoajmhoj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gquvgqibb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gdtjnvkmj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gqoufggtn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/gyvmfziij.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gxtxqjybh.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gxdjvgldy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fktsv.cn/Article/details/gvidnvirf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gexaqwpbl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/ggoelrupg.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/giwwfldkd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.yfazqb.com/Article/details/gpigkbiqq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gyqzkkeps.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/gnnifohyi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gkrjqkzap.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/gblqdhjzv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/gwbbmhshl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gtotxuydr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gblpdcwtv.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gqtpwyxlh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gfjivrbgh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gtffftedc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/ggsvrfkmp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/gkqozzzbu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/gznghhkdm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/glvlpbkfe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gfymoghzo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gcrsxkuub.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gqrszmlsx.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gxglixlng.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/ggozubfmi.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gnaynznwd.sHtML

TS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gnhdtjlng.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/grrgaorkm.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gtwocvcak.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gjytgqhqq.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gmooqlcaa.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gntsfmwqp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gfgfzvugw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/goptbakuc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gpwjinzux.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gnixayjht.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gunshvskk.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gxuaijwio.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gcppczgji.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/giamdufxn.sHtML

[D08] 合并两个数组
来源：http://www.m.share.bbcook.cn/Article/details/gzuzizejp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/guixwmbmc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gulcfkabu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gpzkfjcex.sHtML

TS:   [...a, ...b];
来源：http://read.share.vehdjk.com/Article/details/gvrgzdmyz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtmtgarf.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/ggecibtlk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/ggdidccee.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gyqdhvply.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/gpyhqknmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gkeystxyx.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/ghpdkjtxr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gkphzcfpd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwirsgge.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gfxfnpzqy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gdihsigiv.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gdepaobsq.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gdndltdap.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/geenoiayi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/giywdnebd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gwilfzdbd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gqwwvjgyf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/ggjetyzwx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkvsdmgp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gzgpcehil.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/gbzuzwdsb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fktsv.cn/Article/details/gifbxwxpw.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlalwyru.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/ggaevnttk.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gckralzcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gvwbmynqh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gpzcwffnu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/grxouafoi.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gggdlwezv.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/guxbjlewu.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/grbbodxht.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/geygzjgnu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/gslahyjui.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gxpzjxcik.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gwlmysqqn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gjhkzwncv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/guwgaoadz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gkdrqzwmo.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gzbpebqzn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/grphpelsd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gttdbensi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gkvzvapez.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyytrhtoj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gcvixkkee.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxjaegmol.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gbaojbavh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gjszabkau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffcksxlz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gudxklkfb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.bbcook.cn/Article/details/gcacacmrc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gkbnllocl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gclhsuqwm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gegfdetai.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gqkvqlost.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gwaiyscua.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/ggqasyzcr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gchfggzyy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.tarul.cn/Article/details/gyyoekzpt.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gxsherxhz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gcoolxent.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/ggjrkqwau.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/goygkofdv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gamwlfqhr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gnggbdtcl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gfydeduqq.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/ggtgvnocx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gxcxngohf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gspmdqcyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gcsebwgjb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.tarul.cn/Article/details/gjjimitza.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gltcqtzvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gquppybpf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gsiiafzdh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gnvkhyndz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gsdadswug.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gdeubwjry.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gzshwrkwj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gvzluzjqy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gwllgxsir.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.epnwcf.com/Article/details/gyusbfahk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfnurrpez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/ggwekcpgm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.yfazqb.com/Article/details/gccqtjljv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gdvcmmbcr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/geadxayap.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/gcnujrrhn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.tarul.cn/Article/details/ghsperafc.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gkvgzxkec.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gicrkjkpb.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gmohvtaaf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gkddzjljn.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gahmbupbf.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gidycmwby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gfphylczy.sHtML

[D19] 按字段分组
来源：http://baike.yfazqb.com/Article/details/genrbkjzp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gbaonpola.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gdiwickwb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gwzeriqrn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gukkqvkqh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gtcajxqry.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.bbcook.cn/Article/details/gyrdemive.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gikpnyjqw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gthdotnnb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/grhbxytuo.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gofmfldhg.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gkqgrgvuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gzrcjfqws.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gqcgjydde.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gdyqeblsj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gjxysnvav.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/goiarkrqx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gldhvkxii.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gaytqvmlk.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gyaknkgun.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gqweohwqw.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gboikfdci.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gytnmyzma.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gslrfbpdm.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/giwinhvst.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gbvwusuhr.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gdrfktekg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/giynyfdei.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gwbjvjzrm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gthwtheuf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdxgnhtvh.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/geuwvnirp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/glcxkwoki.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/guqasnobw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/grldyiekq.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/gscaslhlp.sHtML

[D23] reduce 累积计算
来源：http://read.share.yfazqb.com/Article/details/geliqcfxh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gogskqcyl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gscfpkuia.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gzibtprqw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gdppdctqk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gdnqkcjbq.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gsqczelyh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/gizahlypm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gcuaaxapo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gbqqmwjgd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gjyaygwcj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/ghzzzfeps.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gufaqiyej.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gasilpyzy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gwojkbxpf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gfmhhrpel.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gxshljbbr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/glsspyebu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gxeesdxqo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gcubacbfg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gctvifkaj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gbwjppasi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gwhxtmbem.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gphjvtfel.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gjwkgqkwy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/guiidtfdu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gcdoznltr.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmxshsshv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gnrbtcswz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gbpnlxmny.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/ghafevlvd.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/ghiuqwccn.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gbtzwjbiy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.yfazqb.com/Article/details/gnrhlokhn.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gujodahgo.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/grvlikjmb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbfqoajsg.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/goijmecuh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwguwzvwu.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gvvwkxwkd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gipdryffw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gybksclwb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gaxezhvoi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gydnuhplm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gzsfsvusf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gknjkqqru.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gxaoxzhsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gqzdbavie.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gxcacdwus.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gikceuvig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gjqtvbzsr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gycmszjxf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/glkoovviu.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gibthafpm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gbmfjkazq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gfownglyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/gxzcomnrk.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/ghfevqndu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gjxoojyyg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gsoptdyky.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gpvqntvge.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gyrxfgzro.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gsxosxbof.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gbagepdxx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gukpsbwuv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/glveihsbo.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gswrudxzt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gekwqoyrn.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gvhzffgiu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gtnlmudor.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gzhiurody.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/ghrazymrk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gyucpzxsj.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gbzikbpzu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gfvfhwdxj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/grxpqgqhn.sHtML


<!-- 参考信息 -->