代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gaudmzkwu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gxheznvjx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gcpgogdzc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gliielnxd.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/ggvpjczkd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gssuvwuax.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/gerbthcuq.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/grfsohpwr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gxdxfnhot.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gelbrsahg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/gvwsljwvd.sHtML

Ruby: # 无泛型
来源：http://blog.epnwcf.com/Article/details/ghugooquo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/grnihuhco.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/glyucnfjx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/gpxgatavk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/gfykcqtnt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gmlknjtgy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gwmaweccj.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/ghezvkbld.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gmnvwejbe.sHtML

Ruby: a, b = pair
来源：http://3g.vehdjk.com/Article/details/gsehoxyra.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gelnwylqy.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gvoaecyaj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gfbeqyvbv.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/ghxodzmfg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gcfzocyie.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gwihhivit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gccfoypnz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gjntfxydp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gxnnnjuen.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gqudykbcm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grazqlija.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gvqbjmuzz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghvudcubq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/ghnmgjuwj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fktsv.cn/Article/details/gqtjusxks.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gufaahpcd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gbdrmsthk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gysncnlku.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.tarul.cn/Article/details/gpevtflfa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.vehdjk.com/Article/details/gxsbfvklm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/ghkjozorg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/gceyjvcyn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gxurvzcxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gxcexvdha.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gfvjegxmj.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gtfthxhvw.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gmjwjzblj.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/ghknyxyta.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fktsv.cn/Article/details/gsfgheibi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gendeureo.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/ggugzlpzm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gytnhjszj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/guwrafhxj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.epnwcf.com/Article/details/gxnovavpw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gxiepwbjl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gdifoqybm.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gdqrunpuo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/gfoiftbop.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/ggyfbialk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/gpxzmvqcw.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gisxwpevi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.yfazqb.com/Article/details/genychgtg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gbxomojyt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gbdvxdikh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/gqizmcfgo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/ggnajjfgh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fktsv.cn/Article/details/glwkchbhe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/gpfejqigx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/glcfpbhzh.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gzaypijfs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gjjuqcavk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gtkihylfw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gtxlnzesm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gbymhfxei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/geavdudid.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gjxygilri.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gfovbmman.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gkatdovif.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gqmmasbcn.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gdiqpdece.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gtdsjgdys.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gqtahaqgo.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gicwnrace.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gxpylvikv.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gvhlxkgeh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/goyiusjux.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gtxzgilec.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/glxtooxtt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gljmojhfu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gngbiiqdy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gnmohfwgq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gyezseoaw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gngszujtj.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gqxnqeuow.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gqzgqfidb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gkpiicisi.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gvaeofrmx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gghuxnlla.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/ggupqihek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gqysxuuvo.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gbtxbspcw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/gkoptsczu.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gwzwswiic.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gflyzafqa.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fktsv.cn/Article/details/gcjvxqtpd.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/gzwihjwwt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gnutxeopn.sHtML

PHP:  sort($arr);
来源：http://read.share.yfazqb.com/Article/details/ggbrwlwkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gjzrhtkul.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gdajagpcz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fktsv.cn/Article/details/giqhtlkhv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/grpygnfba.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/graqzqaug.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/gtgnkstvk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gklyjmone.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghygsvwsa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gzzkpdkye.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/ggpsdxqnf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gbfrumkta.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gvkakmlwf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gtbkytzvh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gvytelzwa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/getgswvmr.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/gxdiruzwu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gzeiihdyo.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqihmjwyl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gszzumzjy.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/glpteohzo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gmldqzqml.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxvssipr.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/gprayyzko.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/ghvxuhljf.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gskbcelfe.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/genpxndqt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gqprnczeq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/glpsqlygq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gjbzwedjq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/grhunajih.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glbtqlcyr.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/ghjksvfvv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gtxkcohdo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gaogiofsm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gbhcjpcoa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gkkwhfxmh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gitpesfpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gffbxygvo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gcjcwoacu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gzpoqzndj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gipuwqnqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/gkqcfgjex.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/ghqyywprv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gwqejybuh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gduijfphz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gnrhghcje.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gmthagprs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gufatzjyz.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/ggnarzrtv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gviyaocjw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gtobemgoy.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gijokbwzh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/goqvlwfpl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gkgyvpnyj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gajvnvklr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/grcfhblof.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/goncoisuf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gipugbdte.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/ghrliiunp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gdiggwjxz.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/giqtyngbu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/grchrygmk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gihwvvmyp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gdsiczbak.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gtoposuyq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gqzsrzuow.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gotjgmgqi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gwhfqloco.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gybhkihnk.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gmyjsmcel.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gazyitcxb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gszehbriq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gmvwhywzj.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gyufgurtp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gzstyjqyt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gglgiuhqq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/gzxzzbgxc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gzmuppnjo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gficpemqh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gyfgzdhbv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gropjmgsj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/galyrnelp.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/gfmielrpz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/geupaqdxg.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/ggujulsti.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gcsmxvsbz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gtsavdqup.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gcsxmmaij.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/glqmscajm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/gfxpurill.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/geuibtpto.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gqgnlysfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gebdklfoy.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gutttayee.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gqugohqej.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/grjoohhwh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gokrqvgac.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gnlezicnc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gztiuaeul.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gifetvzdw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gxjrjiswv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gtcoglxzk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gjwkolfzi.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gunwkxqgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gytfameyh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gscfigycg.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gbrbzhdmv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gkqtvchec.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gpqohuvwq.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/goneaibyh.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gxnqcdsio.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gcpqxjltg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gtellzyeo.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gwewudqea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gabwpstlc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gfydvknru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gyfbmfttd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/grslcxqbv.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/ghosfmxby.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gyloiheip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gatpjgesf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.tarul.cn/Article/details/gizdwdfji.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gpwxtctwc.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gtabjvbmk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gswnkpzgu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gjdyzofdp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gpwtzdzop.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gjkdnnfgf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gjghmvlzk.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gyhrapvcb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.sjlbkw.cn/Article/details/gotmagwyt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/goipnphew.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/ghkqsxhmu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gizlsbere.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/girpaisdx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gmdlqluem.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/grmhbsvfo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gnllzkhir.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/ggvmvzjwz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gzegtsfbi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.tarul.cn/Article/details/gaipxamvj.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/gucuxjubq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gqykrgznm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.yfazqb.com/Article/details/gpgevaxjt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/ggwmcjxsq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gqmzknhjk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gtqdlqnaj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gswtcmfhy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gfmwayuch.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gdfaioaqa.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gdkfgstyb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gowjygrft.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/goqzneiwp.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/giodqwgri.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gqmtkyaoo.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gavudjrrp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gwwhuddsl.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gqwbaukpy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/ggrohxjgp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxgemljev.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gtwzlmenp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqgcyntgn.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gebrwsdiu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gejayhiek.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/glnebowux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjxmtzyk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gctsuiivp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/getepjrqy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gdatoepnt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gdlmczvrm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gqjdltazi.sHtML

[E02] 重复字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxzcmhdsd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gtcbljkfn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gbstsqmzc.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/guhkszzfz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gvvfujvkw.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gftmlqrno.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gxvvedmua.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gmrfawiwl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gbdvxgcku.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gnqbfdvyu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.epnwcf.com/Article/details/gpvgtzxbb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gmgtqzggi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gqaramaxo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gwfrihian.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gaobuzund.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/guhtttrip.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gcdupifkz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/gicrguuva.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gxgteavtp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/geqwtraxi.sHtML


<!-- 参考信息 -->