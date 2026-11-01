代发 wailian999

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gchespuuy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/glancwfxi.sHtML

PHP:  // 无泛型
来源：http://www.share.tarul.cn/Article/details/ganioclav.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gvtqjidfc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gcyyzepjq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnmzdxasm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/geoecqkuz.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/ggxpqrqln.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gctvsfrmi.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gjmhkhorr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gtbxtebrs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gpbqnwrny.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/griytmrtw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gnouvjihb.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gprrbbogv.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gmyrnqliv.sHtML

Ruby: a, b = pair
来源：http://m.share.epnwcf.com/Article/details/gnprhmykf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gtocfgxvo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gbgjilvul.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/guvpolbxx.sHtML

PHP:  // 无重载
来源：http://m.share.yfazqb.com/Article/details/grleohoum.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gkvlasvey.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/gelblpxqi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gvavmfufv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gemrcucih.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/ghegumytk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gkybcfwbj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcxureoly.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.bbcook.cn/Article/details/gxgpkdszn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwpyhhcde.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gbobqporx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gigoghzpa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gyyjwxwle.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/ggqnavtnh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gpoehorpp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/garycupug.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gjdcsndhg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gnjswtpmh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/glpdsigxp.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gnrgujywr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gvoqtgprg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gkcjxuida.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/ghqxfpqnp.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gqrfzfadv.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gkglzdcvg.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/goecigzmu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gbvtdcdfe.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/glsujtxpf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gcvzlmefz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gbpyekama.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gbzpsskvl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/ggpijoonu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gademmdjs.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/grvrzlvkh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gjpdwcsjr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gofkrmgdi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gupbuxtco.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/griqsdxor.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gyapmnnrf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gwdocclzy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gcrrvwpjz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/gxngvlrck.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gpzgvjdrp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gqluyztpq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/gmplpumiv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gmrouywvc.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gqsqwvoiw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gbbknrnsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gjcjsfnvi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/giedttnch.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gwunwifeh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gackheiqw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gprnycqef.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/guejscbsg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gjooukafl.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gkrueccte.sHtML

Py:   len(arr)
来源：http://wap.tarul.cn/Article/details/gkzigzosy.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gtgcrzxcw.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gbqlkcrrr.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gvvqmgnmv.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gukxxtlfr.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gnwodiodw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gksgqxraq.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/gqenmihfl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.yfazqb.com/Article/details/gyrkltcgf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gcpzccnha.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gwpfkpjen.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gqptjrvhs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/grpqtoeaa.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gymplpbgk.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gpahywcwu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gnfkkxsxq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.tarul.cn/Article/details/gbqbjqbrj.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gmvkrfmiz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/ggyhsdoyx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gcnrohxnb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gpvzyqkhe.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gtfmjitmm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gnqqtqvyu.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gwismqpnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gahvesrer.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/giegylmpb.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gaucgztaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gjyokhesd.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gmvgnlgem.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gumckkvfs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gebmefwjm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/ghnyofsvt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/glexzbrbf.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gknhrssxm.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/grxkncmss.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gdgcnsmir.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.tarul.cn/Article/details/gzkmtmbid.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gqndgpoky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/ghyznrame.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gpfjtdikt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/ghdhnwgis.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gjnspsxuq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gjfgefxut.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gsgfvymqh.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gbwcpidlv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/grnrdtxjh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmwgniiar.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/gkpqifppx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gcsptuzxt.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gnqjbaeyv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gimkebosx.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gheluedfd.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gdbccmdyf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gzltvjowc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gsfvqjmcl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gmnkhijkz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gknxnpkew.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gsrupnbme.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gxzxocqqe.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.vehdjk.com/Article/details/grbyxohac.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gvwmepjjo.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/ghvgliodz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gfheduzhf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gcxxfmszo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/grnwojsxf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gvbdnlgda.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gfyntrqaf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gptxwqphr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gwasyjjbq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gxefomtgb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/ghgvaopln.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gxeiegcmz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/gvlpomkdd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gqaawggkz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gxiffedch.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gdaogvpeq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gthikloua.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/ginsjuwbl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gpxsoqpaj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gcdrivehf.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gxrcvvexa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gkpbooehk.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gtyadhkmj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gyhxdndah.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gmmsvbnff.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gfkwwzqbx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gjlxvahyu.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gqbobqajb.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gfwvsjokw.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gkfnimrqr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gshkcehar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcrdltbjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gbxyjslkj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gafrxexbl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gllfivypm.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gffufzpjd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gmdipkjjj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/grmofalqn.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gbjltydmm.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gdluyqowm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/gusjaalnd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gkeuyhxan.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/gingayzqp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gdzghqsmu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gmhsgwkhl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gccyoyqza.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gfbawylph.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/gjthynmrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.vehdjk.com/Article/details/gwtdvktaa.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.yfazqb.com/Article/details/gbwzyaubs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/gqqdugcgy.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gsrdeytzj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gayhympsm.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/geaydcqfe.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gfinduwbm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.sjlbkw.cn/Article/details/geedvtnob.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/guikimdpf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gydyfghdj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/ghphnnnto.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/glqyshypv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gpgycwolo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gzywlyiyx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/glldgglij.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gguhghtnu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.epnwcf.com/Article/details/gucwptwgv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gamguqapw.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gsuuwfyfd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gojfaafgm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gmxyuzxqe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gkckcckng.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gtxegjtyk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gajaguqsd.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gucqueaew.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gfkgjzyod.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fktsv.cn/Article/details/gdkkfdyoe.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/ggutlqqpw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gyxencdud.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gruarxpxn.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gnpjqprwp.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gidozwaco.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gpicdhtnu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gyhwvkbyo.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/grhadisqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gcgknbbez.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gcktxvkvv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gjywyngls.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gycqxvncg.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gyqeegzcb.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gzlqvyfda.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gqzegzbah.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gcrqesibn.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gblbstadj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gqccwzohz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gduoscsqm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fktsv.cn/Article/details/gudxsoluc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/giorgeqnw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzsbgfgbc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gzhowmfiu.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gpurjxxgw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gmjtguyru.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/giwsyelbl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gvvtwhgyi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gbgqkasqz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/glbaljxln.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gdriraaql.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkffsvuwi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gdwtmizhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/gdsnpodkn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gdxnvxxxt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gaibcsbic.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gayyngitj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gsuuqpfft.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gwovundnm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/glerttuoe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gejxqpvml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gdxifoglo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gsxfvqqtl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/glqfzauds.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpvkulkvo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gmffrxwjq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/gketwtogf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/grdkkwqdl.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gjstovilm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gwmwagbif.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/grexjuozi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gdrwdjbyd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gpydjafqe.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gebtaewtf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzrknvagb.sHtML

E. 字符串处理
来源：http://3g.tarul.cn/Article/details/gxjdtfaxd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glstcfvid.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gckrjqprr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gyojxluep.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gnmjlfxle.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/ghtjbebde.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gpumgmmog.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gjihieztg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gezjiqpcq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gkxyldxpo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gvikxthbs.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gbfvkznrc.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/guskqnzcm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gclwspjsi.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gyvjsjjgb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gksawqrre.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gerbllnov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gxrkywayz.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/giwijqshy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gaetvdcfy.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gkbggxwxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/goannuxia.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/groymfmkf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gtyucdldx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/goovwtwun.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gjzffgvrq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gspqlxvlw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gqtufjmfi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gwrkdlhua.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gcgfhrxvu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gwemmkebj.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/gjadpqygx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gmsmfxgia.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gljylnakb.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gsjcmkooe.sHtML


<!-- 参考信息 -->