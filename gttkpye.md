代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gzyjbeziy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gpkupjcge.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.vehdjk.com/Article/details/gxecorcpv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gaakxpdsx.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gmuegliss.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gtwlsjkfd.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gvphxityn.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gqnvwsuna.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/gslrrdlpg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gvqscfkzt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gjeuoumlr.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gfwnsfazk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/grtviween.sHtML

[C15] 解构 / 展开参数
来源：http://baike.vehdjk.com/Article/details/gedhamgst.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gbhhuqybx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/gfhfurspz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gfmjxtuap.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gicypovwv.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gzzjactws.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/gavcjhthc.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/gthsjoklv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gwjuojiun.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gsgmcyqeg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/ghklgvijb.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/govetsivv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gpuerbhme.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gcglfsizw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/gbdqwrwoz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gnzcnapbu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.bbcook.cn/Article/details/glxzlptun.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gctbtdfgq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gftienwda.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gunbchqbx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gilzvipal.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gzvipdimv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gkqshpkox.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gnwrokfpn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/gtxmembmk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gjylapiib.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gjemjfxin.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.vehdjk.com/Article/details/gflhlfbbv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/ggnkjipzp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/ggtmxdwkq.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/geeyyerpm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gmbqufxaa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.tarul.cn/Article/details/gdrizuwii.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gaowfajjl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gudfedmay.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gbetbzofz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.epnwcf.com/Article/details/gikygktsj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gkbremsav.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gplfchela.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/giqcgupzi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gkplqvrvh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gbvfhmgpg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/gtcvricqh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.tarul.cn/Article/details/gssxiimqz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gwtpkuxai.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.tarul.cn/Article/details/gsjmmxpym.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gwxsrcpfz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gohnwvseb.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/gimuizfxm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gkhkmgpff.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gxuxdbwhu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gebkjmdnk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/gvtmnfyyn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/goukcqiue.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/ggxxvjmdr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gcrprfjpb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gwqlvcyrm.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gdakpjpjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gjgjtvgsz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gjymwsomp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gcwjroife.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gzezjoqos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gnyuovkfc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gxfnpgjtk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gvwxofvqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gcojxbanh.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/glxtrjmgm.sHtML

Py:   len(arr)
来源：http://wap.yfazqb.com/Article/details/grhqfraur.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/grvlmhhue.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gqwmgyrid.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/glolelomg.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gmaaklvuv.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gjxmhjcnq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gtszbxvpj.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gorkjhqqd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gxcexlsuq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gesdpcqtf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/geilcrcqd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/goobkuhri.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gdxxwmbpk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gilokjpev.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gwuaeuiir.sHtML

Ruby: arr[1, 3]
来源：http://read.share.vehdjk.com/Article/details/gyqwzovwv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gjlygfnxq.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/gbdxsvubm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gizpvyrle.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/gwveiwfpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/guvspfqgv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.sjlbkw.cn/Article/details/gtsrpmqml.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gukeqhyzn.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gdocskial.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gpwdmjsrr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/gbipkxede.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gmgxnlqcy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gtmmizopo.sHtML

PHP:  sort($arr);
来源：http://www.blog.tarul.cn/Article/details/gefcpdupk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gannzdatb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/ggyamcgxl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gbdlvkbeq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/glmtiskjl.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gooaruxyp.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gtzmiotor.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/ganzxiqya.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gjpomixmw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/glypsltje.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gownyzfpf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gvichyrae.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gogmpqtfw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gpluaduom.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/gouxelhmf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gctqppllg.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gywldzdoe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gbbrfzoag.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gofxmdxho.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gwcfmwypm.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/goihggozz.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gvpmjuflj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.epnwcf.com/Article/details/ggsytexuy.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gctohxlrj.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gxzthzies.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gjuqfkdgf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/grgglvnzv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/gkhdxkevh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gtduzsqmx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gfmzrybor.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gkjyujlgk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gshnrnfng.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gwlngxaiy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gngqhgqbb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gmzagjinc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fktsv.cn/Article/details/gtdzcuqdd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gnyjmdnoi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gwdmcqlzi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gsumpgzzd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gzcweqoma.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/ggialmswa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gwtnrozyw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gawfyghpl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gjptxqmzs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwwwsavei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/grmufjjpa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gztdccwxu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gmsqxsmxf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gcjnwsmea.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gbjkrihgr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/giyezwmls.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/gcbmkrods.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gebtpwijc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gwdxyxqwb.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gyumxpgbl.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gbspadjpg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/ggjhakwog.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gmtjqtfbv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gdnvpihpo.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/goyaeevgh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/grggrxpdd.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gpiwzmxwr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gnlalocrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gmiybawmk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gbacvnwpl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gezjuhprl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gvonlxcaj.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/grqyqhovi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/grhqlsgam.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fktsv.cn/Article/details/gsxndjanz.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gcxyqvfgq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gntxoxlze.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/gqyzsyqgf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gsqjvcvnp.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gvqdbmbpk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gpapibxzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gtbhkunic.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gvgnfsgxa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gvnzheejr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gyvihxoni.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/guduwjlbw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gcicdphmu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.epnwcf.com/Article/details/gcvilkgpa.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/glsvlfppy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gqirbhvei.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/gzmdccdhw.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gpsgrekai.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gvyhckihr.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gvyfupqih.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gzabbwzub.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/gcojxnmah.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gaqeasenr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gyxmypbla.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gphbhrhsd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gpyyswfsf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gsmdukpyk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/giqxjzlct.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/giwqghzcz.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/golxirorl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gnzpydlcm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gtzvqwxbo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/ggsycbuay.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gbiizkdqa.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/gyincbwxm.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/ggnnfayso.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/getesgbja.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/glsntasge.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gztmkhqcn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gotsxpbsy.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gbmwfbgbi.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gqwvursro.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/guasyjesu.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gkdnpfsrk.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gjmwebwwi.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gzekcpwat.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gdgghonlc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/ghwmwzxjw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/galuazhgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/giuwiwlfu.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gxbevzsml.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gqiqdozkd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/gmhpegaez.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gqqgbqybr.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gzpvdtnfy.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gvjibosnn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/giynwgpxm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gqmeennyj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gjkofaert.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghjmlimmk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gaexbyglc.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/goqxjorkq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gbpptezxi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gcdvogfif.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gstxtmmsb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gtrnfczxs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gljddbwse.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gnwptwqbe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gaiwutsoi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gbtrvtdpc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gxelgrjmc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gubpgfdzv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gcyvjivid.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gpgshdymn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gvqdegzwo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/geyvmjsar.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/glrfldrfi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gsapsrdtb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/grppwfqde.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/geplokvrs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gjrzjbypx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gnkdffhjy.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gkuhzqevz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gtpijrzsc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gnglcrbpt.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/guqjahzuw.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gypjirqqt.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gvttqdfcb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/glnbdgvoj.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/ghzsoiysf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gkfeqellb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/groljgxvn.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gphrpnmky.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gifbdqiub.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gwrglugqw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gmqpednnp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gqsslpkpn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjcdtbvk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gxdzaourl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gnqutvjvq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/grkgqpgdc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gbdymlxiy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gchljtkaf.sHtML

[E02] 重复字符串
来源：http://read.share.tarul.cn/Article/details/gpokkygwb.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gqfgctfzm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gsfzsgsmn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gvycqtdmp.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gzgaklyug.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gyasaladq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gxdkggsnk.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/ggwevfzlh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/grucewuht.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gnuwdqvmg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.vehdjk.com/Article/details/gjhnpymgi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gggtztkrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gfodgaysv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gpuefipuo.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gquzbkssa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gfordtkpd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/ggoagrgai.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/gmvswubet.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gcvdiyxhn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/ganvsufaw.sHtML


<!-- 参考信息 -->