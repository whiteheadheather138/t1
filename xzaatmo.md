代发 wailian999

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gsotpezfu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gfdzkunwa.sHtML

PHP:  // 无泛型
来源：http://read.share.epnwcf.com/Article/details/godegvavj.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/grydtmnew.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gsvlvvfsp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gsugnfwew.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gvdqrwpsw.sHtML

Ruby: # 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gdxqsngzr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.tarul.cn/Article/details/gccbfadar.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gfaudmllj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/ggrkldufv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gkjkuzqqv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gpykkpvrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.epnwcf.com/Article/details/gdizznmvx.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gznwqfayt.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gojthzjms.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/genpdtmft.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gsfbnwfpq.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gvwnuuulp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/grqzxxuhr.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/gxlycmfog.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gnxirdyey.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gvgtgirkh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gddhjhubk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/gcqtvfkqa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.sjlbkw.cn/Article/details/gymrqnyzc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gydpxtecg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnjpqxycp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gqxwnqrbf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzkyknmfv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gnwaiixqs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gwassjtri.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gsywkbgvh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.bbcook.cn/Article/details/gzphmlxvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gtyuxssuk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.yfazqb.com/Article/details/ggftjcpcu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gltrkyenu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gggtvgero.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gfpjuefwe.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gwznnqjik.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.bbcook.cn/Article/details/gjteonpiv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gojuyjumy.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gaphavmru.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gdwtxcljj.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gbpouibyn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gajidpqdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gybzbvdyo.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/grihywmfo.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/gqvaqieoy.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gbvhjbntv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gwsjwwoci.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gtocmkzfi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gswyzkike.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gpzradhph.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gitnmfdmr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gajidgsih.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/goxgxyutp.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gkvbvobyy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gvqvvaxpn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gbybofekz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/guhewahcy.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/glheichki.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gnelynuev.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.tarul.cn/Article/details/glrfmznym.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gfewzqfar.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtmteukd.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gsxplyaer.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gsuanaxux.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gnzxzkiwy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gdahzydbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/ggaosrgej.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gscjxjywf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gurlfhaqc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gfltaodqe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gsocqnbqx.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/giercqkmg.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/grdegghkq.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gxfmscota.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gdzgojito.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gvxdfvcsg.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gsnkaetoz.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gvtpydnal.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/glridmses.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gbtonxmjf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/ggyhltsks.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gbyzfgcfa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/ghisjwtbb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gypaeqefk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gjbxqauks.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gunuzvwyt.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gybyyablo.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/ghwgzngwd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/guvnohcwe.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gfqiuaool.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/ggharqjns.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/gcxvobyag.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gblzpqqva.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gipeygwfl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/glffguptn.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gkwheahin.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.tarul.cn/Article/details/gsqqnyctg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gmijoqvnu.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/ggrubfbeo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gjlvdxxzx.sHtML

PHP:  sort($arr);
来源：http://blog.bbcook.cn/Article/details/gfamhnzur.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gymuogpuq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gwyzxluqg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gkvthxbzu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gsihcabzk.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gnimemcyp.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gefnbwbtz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/gatkhtpmu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gryvzhidc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gjcrwxabo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/giwphxdks.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gdlpottyf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/grjjbmfbq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.yfazqb.com/Article/details/gpokvpydn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.sjlbkw.cn/Article/details/garjwdqyy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gdswakdps.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gkphqcwut.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gbtxcsqku.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/glaxipzro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gaobvskmy.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/gfsdxrtkv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gbjnsksna.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gkzktncyw.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gltheihpn.sHtML

C#:   list.Reverse();
来源：http://read.share.bbcook.cn/Article/details/ggvitccmw.sHtML

[D12] 查找元素下标
来源：http://mobile.tarul.cn/Article/details/gabpqyowx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gkblwwsxw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gemkgxvat.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gvdcpqdes.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gdlhfhfpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gxyzmvonh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzuwedxa.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gwjybbqfs.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/grupzsqdb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gdbbjquzg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gtbyysdwu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gogigdvpa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gwvmxaxho.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gjqmihksx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/guirvssgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.yfazqb.com/Article/details/grpgssogk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/glqouuoqs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gzlfohlgx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gavozeeyt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gmsnuohwr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gfatbtekl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gphperzxc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gelqmtxjj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gzrucnreb.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gxvxfryjd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gtwdparip.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.vehdjk.com/Article/details/gzrzdczeb.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gopksnmib.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/giklbabre.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/ghfvatnyr.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gphdwgevv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gbcxxadtz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gjpsuroce.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gnsbpoumq.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gudjkdupc.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gqffrtvpz.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/ghuxqywop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gspgalzgq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gjquovzko.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gaqcgyenf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gamyepziv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gsprdkswo.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/goauqifvi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gkjtybzad.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gfuzhspqp.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/giwvtifcm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/glqjxhijb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gnkkrqcna.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gvihyjoud.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gxfvbhkak.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gwklgirwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gsckfdgbu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gumtacaeh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gqwetwcow.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gxdvanmev.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gpiroitjf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/glxekfbnq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/glzmorthv.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gsmlmaooq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/gnrvluizv.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gdtkersyy.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gjmeeayoy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gqcxmsidz.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gkubsdjlb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gqkztkblo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gzguhtaut.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlsghjsx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gxgerkgkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/gtnfzvcve.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gkdbrrpgn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gtidgzhjo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/gjmxuktjg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/grcazlxzf.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/ghhsnyury.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gprtluejf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/grindecye.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/glbbtznya.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/goziokfqv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gkssnqpyi.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gvwucoczn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnwrjqsi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/gswjobhcj.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gjwyazght.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.vehdjk.com/Article/details/gpeowoxyn.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/godjqqcqc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gmvmzyznl.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gxlggrzhv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/glotebaot.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gnzznbpmo.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gnhalfghh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gqxkdxuxg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gmawccvkj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gubzbmqzb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/getivrtnx.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/glvoxxdhu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/ggaaardkd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gwgkoeker.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/ghnazqbfn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gawjkzrmg.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gzhpcwovz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gwtzzuskb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gcgebreyf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/ggsqzxmmw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gckrejaob.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gvozwiyay.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gulnevbpi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/glpuowqbf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gokzvdbas.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gdbagearc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gyerpsjcr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gtrdnmzjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gysvgwfet.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gyyafnrte.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/goiqnrrlq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gxfigdqgf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gzcddvxty.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gmybtcxaj.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gwxmjhltd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gbzhzvzuc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/ghyenkiyu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gukiyyqzs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gnsfomhbx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gniliykxx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/grcnwnbdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gkeyappgn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/ggsvhwmti.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gsjennlfv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gjdnsvayj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gnatlfnhq.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gqgpynxen.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gtqwhungz.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gpuljumwc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gzkezjsvd.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gljdbvrqx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/glrxzjicg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpzwpfusy.sHtML

E. 字符串处理
来源：http://m.share.bbcook.cn/Article/details/glbuxrtrd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glglxxoyv.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gtzwhmfwj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.sjlbkw.cn/Article/details/golankpgq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/ghqdcysul.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gcmwnngow.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gsiqhrwjl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gytguywsx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gbgxclrrq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gnpapjpac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gfdihmjxy.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/gobizejdn.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gckbzlmdm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gztrspgre.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/grxwdxopo.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gjrwfulbp.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gozzdsvxq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/glyrxmlgs.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gfhxxettv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gscpoopyg.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvktqzlt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/glrwrvybz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gumgmonuz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/ghkmaezxk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/grwpotyrh.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/glkraxfqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gfodihonb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gfuemlrbn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/goimbdbjh.sHtML

[E04] 查找子串位置
来源：http://mobile.vehdjk.com/Article/details/gyhvcnwnc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gqccxzqlh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/gvcernvdt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gxtyrphwk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gkqoouwkz.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gjoeggahh.sHtML


<!-- 参考信息 -->