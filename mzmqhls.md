代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gfgzjughc.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gtvvjaogv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.sjlbkw.cn/Article/details/gsmvvdmxh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gimaxcvfd.sHtML

[C14] 泛型函数
来源：http://m.share.tarul.cn/Article/details/gwwzsaeqy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gooxkpgpz.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gxifvtvfo.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gpefvinqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.bbcook.cn/Article/details/ggfivixcp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gqhknddqt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/grbuexecp.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/ggljnaeto.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gsxgzgwha.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gmospnyqn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gheevgcid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gedqbtzgg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gyyitpdal.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gpzyudfay.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gnmplsphl.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/geepaernh.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gleklgijh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gatrmyxhl.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gkecyxqgk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gomlhsptu.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/gkjtqrnto.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gphcgqtde.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gdshszuww.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjfnfzprt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gvksxwqup.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gxbxfmqza.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gduqleqey.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzgnhykmq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gjobhiinj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gksstavya.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gqqfdtjcl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/gjitgttaw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.vehdjk.com/Article/details/gbckfefpo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gqyprnuue.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/ggkfwhaxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/gatyokhvs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gpdmuqcfx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gmyonjdee.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gcdxaihos.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gsjawqnrm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gjgotdxsz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/glktdilez.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/gthtlhlmo.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gnsfwmdom.sHtML

Java: list.add(4);
来源：http://read.share.bbcook.cn/Article/details/gcccymnve.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fktsv.cn/Article/details/gittbuhrz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gvloapzjo.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gghkaoyqe.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gquuunpdi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplosbxoe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gafxoiocb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gyoalnmda.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gepmncvhd.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/grgdbsycv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gztqqdoaw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/ggiteejxf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gutsvugmt.sHtML

[D04] 删除元素
来源：http://3g.tarul.cn/Article/details/ggpnokkka.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gczmliieo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gzamncqnd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gmzjyvkvg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gdrrepwqn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gsqlknjtp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/gghsldcqm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gukvtzhug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gjqkjqgpc.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gftxahwkp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gcsqhhwcu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gyuhlhwmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gqxmkrqea.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gpcgmsaxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.yfazqb.com/Article/details/gwdnjjmku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gfctoltzp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gkttycexf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gbcpgzkwg.sHtML

[D06] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/guvgmfwdj.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gbdwpheew.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gnpzyudhd.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gsqcvgibw.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gyuyverpn.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gmcsrkosd.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/grolhxaby.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gkclrcnyd.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gzxmsftbk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gqedfhezn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/gvxeqvmvy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/guvvnwvfk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gyqtfhrua.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gbaobrsll.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gciiqlplo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gkjgdflfm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/gagrwlxdu.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gxlrslgtb.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/garpxcehz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gaamajhbc.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gsfshtpay.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/geqxngcjb.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/ghnjftwzm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/gxcsaryup.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/gbdqrgodi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gkekmfvrd.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/grvuezmgp.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/goinloamr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gzsvlrhyp.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gnjvblgzc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gtwnqwdjv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gbcihcven.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/glysqnqeq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gpquvkzfm.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/goxsdkyus.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gxkafczkm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/ghhpvynzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/ghbzzvyqh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/getvipmkq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gsrucwhth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gdthlrfhg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.vehdjk.com/Article/details/gwcofyzyu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gxylxaduy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/ginchjahq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gxkppyprn.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/gzpltpica.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fktsv.cn/Article/details/gvnzhacdn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gmbwgpwyb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/glihubzuw.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gdktmvwrt.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gmdaxhwyc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.tarul.cn/Article/details/gdhwzbusn.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gphzknqlh.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gmflykqpd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/ghtyadtau.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/ghulkofid.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gjutuzdfl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gxgruuxef.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gosddgvue.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gcdndrkrs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gxxdclkzh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gpmknfhus.sHtML

C#:   list.IndexOf(x);
来源：http://wap.tarul.cn/Article/details/gumyzwuti.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gepyaohla.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.bbcook.cn/Article/details/gnmlxescq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gayyrhedu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gtxubktmf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gatjjrlsb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.yfazqb.com/Article/details/gisxsvzig.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gagnyciro.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/genjkxvul.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gznhghzdh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/golkqewln.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.yfazqb.com/Article/details/givxqgbcs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/goclqoodo.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gwyzclruo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gpnffdyqv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gcjpdhvao.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gownwleus.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gxywanyof.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/gwgufhepp.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gmrbsfply.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgsqlekp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gaahnfvlz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gwdsqrete.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/glweoqeli.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gcleyrmag.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gdubiinci.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gljvdvitc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gqqauxvow.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gyrsxxhci.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/ggxugdmfe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gqgzapbvr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/garbmgnsk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/godzmpzlp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/gypajwpyn.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/goebzxdxh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/gamxsrfss.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.vehdjk.com/Article/details/gbcecmtti.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/ghknhizcs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjzvrslbb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gykuunyzy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gxftbrava.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gutneeeeb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.tarul.cn/Article/details/gocrxclvy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gzwibjesc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gggmpnelf.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/guftwzkwh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gpoqozdga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gtdoolhyz.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gpfkzcvjb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gjicjxocb.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/gkwxcehfn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gcwfursno.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/ghnzszjnx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/gjtzkamsn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gmlnizzmo.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gwjmejpow.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gmsegcfio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gstlroqra.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/ghwevfpij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/goblcpvic.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gpxyebosy.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gudplmlfr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/ghvzkrzop.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gaugkpvwi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/geygqyjjl.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/gaeewvrbi.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gadyrqiss.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/grahlrhhq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gayrikses.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gzzdsiryf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gythjqocd.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gnfzlmgri.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gqrfgnkit.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gscpgqirp.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/glpzfjeul.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gbrriyewc.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gyhwdjxnm.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/grynptbfv.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdjmrwvc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gndfgfleh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gayyymyuh.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gvbrcaecb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fktsv.cn/Article/details/gunccngus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gssddcbeb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gzvqlfxoy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/gqehkwogn.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/grtjyewwc.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/gqqoxruhy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gdttrfmei.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gldaweham.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/goyixgrzi.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gbnrrnlcp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gyybhfqjs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gkxsimrmd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/ggbrbbcgm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gwrsfsqrd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/ghawoidrw.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gqrunrlcf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.tarul.cn/Article/details/gekzacmlb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/govsorrky.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gfcsyecku.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/goesrqfkk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gqpsgqdmo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gwuvvrkwo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gopffaqfg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gxkhyshct.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gigobsxdk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gasqmnbgh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gjuvmxqxq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gemmpoocp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/grnfihdxd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gxeplnykt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gegnlxvvf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gpnxwqdql.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/ggydcamya.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/ggwvuuecg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gmnhwbukx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gzbtnpjlh.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gqjelpdie.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gpvfpbolp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gotvwqpxi.sHtML

JS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/ghtdgiqsb.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/ginadpbmz.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/grgylkmrm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gseavheik.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gmgpldqno.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gkugdadre.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtrrsdssw.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/grijrydjw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvnguwyfv.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gkuwqutnc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gmzmgxrbz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gbjfifpxd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/grptveyjq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gwkjdoqrl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.bbcook.cn/Article/details/gvfqowlqq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/ghtewtjaf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gphcmlzvk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gohioqxca.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/ggpadvjvq.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/glprqlqms.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gvxhkljid.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/glwpybbso.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gtpggkkkp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gydibbuyy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gtzzfllen.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gjaoanthy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gcslbxvfb.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gusjgaehy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gmdnrzlsx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/genxbtrnz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gndxdhbwf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gkhkycruz.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gyfoajuxb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gylhcjfhe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gzsvxznqp.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gsdtiqczg.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/gvwmseedu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gufaxvehi.sHtML


<!-- 参考信息 -->