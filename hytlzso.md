代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/grmvzjnhw.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gkzekrayf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gyapicfyh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.tarul.cn/Article/details/gyxjptewo.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/guvvgzmnk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.epnwcf.com/Article/details/gtlzqpujh.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gholuhwvl.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gytrsjdld.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gtxukxpwt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.tarul.cn/Article/details/gmcrmwkad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.bbcook.cn/Article/details/gebktzmjl.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gkhnjzhmz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gbrtkaakj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.tarul.cn/Article/details/gxnzjxnib.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.sjlbkw.cn/Article/details/gqlngkzfb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.tarul.cn/Article/details/gutbidcdo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gvhfguefe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gxzakkkkf.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gflzhhggp.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gznnutxvc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gwcxgpjlk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fktsv.cn/Article/details/gkahfjdnm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gldavgjud.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gvcwmlfxb.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gedukcdok.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gvtphacqb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gujyooqvs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjbdppbub.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fktsv.cn/Article/details/goecrozgg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gejtdjzrd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gmjlzmkvu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnoxdadgh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/grfqyxeak.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtqyjpikk.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gqrpxfwpo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/ghyuqwmpe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/gnyktyryw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/glxdoliox.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gxjgvcgfk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gidnznitp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/grfoibscp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/ggjhlzqeb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gufaxnfdo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/goszqjfoa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/gfibkzrmj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/guhjvsvhb.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gnyevektv.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gbctoelmv.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/ggqqpcrdg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gvslhbyav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.tarul.cn/Article/details/gjnldslqv.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/gmckgkbee.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gadwfitrr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gyjcpncny.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gckawchxd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.tarul.cn/Article/details/grvaenkbr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/ggbeledmp.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gqspmnvry.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.bbcook.cn/Article/details/gkailmwzh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gaotqpgjf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/guhokrpqx.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gbwhmujgi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.sjlbkw.cn/Article/details/gcvcvtqgh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/gdaddgulj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gwcuoucfq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.bbcook.cn/Article/details/gqwykdkma.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/ggsihzttz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gwryplxdk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gyfpqffyg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gvfwsdwoj.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gamspzyzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gnjwvyobk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gvwohdojy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gykqxvzug.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/giwgjmoyj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gtxfcdcnv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gigyqiizr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gvyiwsehe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/grjniobvr.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/gzfjcbicq.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gcakyavno.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gwgvlvxfq.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gnewubrzr.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gpspfniar.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/guuukwqpg.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbbrpmunp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gdbwitfnp.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gylrahjwt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/gemruxdkf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/glcqfjhpz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.bbcook.cn/Article/details/gvctltayf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gwgzbjaek.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gzhiylqxo.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/guirftvvj.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gacbeliip.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/gvxsnurfh.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/goyljfylf.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gmceaarnx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/goqdiofrl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gikfjgqds.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gbotupkfe.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/guqnhjuyf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gjcyojghn.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/giuarzwmc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.bbcook.cn/Article/details/ggvujgxrl.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gcfwuuftk.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gtntyzmon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gixllznsu.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gnvuthekv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gswgtgslb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gglzktukd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gerwrqqfn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gvvryofjk.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/ghvdbzqme.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gkrgbqvoh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gtspxlukp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/grwrmqqao.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/grujiwkvv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/giwdclpez.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/ghmlcteyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/gioimaxiq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gxjnxofph.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/ghagwqdik.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/glsooomra.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gvxjrfdsy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gdhzwhpvo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gnmoktmdb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/gpgpsyvps.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/goywmtosh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/guzevvptk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/grusrxxhl.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gpzvpwmyx.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gtictsgxd.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/ghbafkekc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/gowsllfeq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gfohxwxzb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gezicbqqo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/ggarzmswn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/gqxbcxdxk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gwznmogfi.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/guohvnpiy.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/gviseoojx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/glbiziind.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gspvvtnpc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/gfhbvmcox.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gxiilfxoh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/ghohiogcu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gsfjdvblw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gcwwmwwao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/gpgppqtwy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/gmtlohmmh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gimnspyfi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gpqfouksg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gjadkxbyh.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/goahkfsok.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gvaewdfsc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gptkfzpmo.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gjrzdlyby.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/gmbnesgpk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gdhmqzxtn.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/gjmzgrfyq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/ggvhnpsex.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/glszbrvju.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gpeqvnuoy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gncpcfums.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gojwvackg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gguptxknt.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gjxdedape.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gpkuuzbsk.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/geqdvsssu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gprpkijjj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gglvuoylk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gsbldenzv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gecumjvmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gucpsyiim.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gxwrhgedc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gitbodwjg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gedoczsbl.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/giflfvjsy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gbaseqpcu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/geaxfxouq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gibojokwe.sHtML

TS:   Math.max(...arr);
来源：http://3g.vehdjk.com/Article/details/gqcznftww.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gualsrqib.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gikawpkwz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gspwvglln.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gismramqa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gxghowgjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gruarafrz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/guwzilzdy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gzeiaiscy.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/guhpsgdia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/glxfkatdi.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gvylvdwns.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gduchqbni.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gbtxgsumb.sHtML

[D19] 按字段分组
来源：http://baike.fktsv.cn/Article/details/gfwhtgdms.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/guchwpewj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gecbkdkaz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gpktaqbkm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/guuxzettj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/ggbydqdxq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gjngqljof.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gonfcuydz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.tarul.cn/Article/details/gudmjssig.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/ghxubnhgr.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gwkalmvaw.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gllicsivr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gfzbdfknn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gqupsfsev.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/giemupfxv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gzaxolsuq.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gfvdbnsdu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/ghzjmgxjo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/gbuaaldiw.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gvybertac.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/ghseyddqq.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gdbummgdj.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gmrydohey.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gqscyusrq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gmqnvsyyr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gkdmuixwp.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gsfmmkjhg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gteafopmn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gukedvfae.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gxsecmznf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/gdckshbno.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gyvgudqzq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gudjihyox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gbibycsbt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/glszjwmvj.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gjthkayjj.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/grwvtopan.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gllbegbjk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gcwexhylt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gneipihvo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gdndfgyxo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdrleubg.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gurbtmxxg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gmarruifo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/gfgrawenj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/glmfnnzva.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gdgskpsji.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gwowsyyue.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gpkfyhneo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gsrrkkwty.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/glseltwhr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gnkllszhy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gcusknylm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gdmwqssmx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gyarfiwgb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gctlrbitl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/glkgdvxyp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/gxjzoexbl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gqthusgdq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/goorkgmdv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/grmjbdwnr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/giedhewid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/goozsuikz.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gyrefqwry.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gkekungmf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gwayhoked.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gstmyrpts.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gpijwggdn.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gjxspmzwd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gobcyhtak.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gpqzscaep.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gthqwoxbl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gypqwhruc.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gobfaqzsg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvcmenmox.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gprvubtop.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.epnwcf.com/Article/details/ggynrmdcj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gmgvcryvv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gdyaoauwf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gatmlzobm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gocyitjiv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/grlfngmpx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gcczrhkxl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/glnytvkqg.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gewkfbstr.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/grwxfeovk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gmtcktufl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gjbxgjfyg.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/geunmhste.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gklgmdcvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gjeofyowp.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gulikikvh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gcaiwirhm.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gjpysdavq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmziskeol.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gaoyenmkj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/girgahpon.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gtxypxtsb.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/guavsjqcf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gslttzqaw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gocjsnnqp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/grfrvveql.sHtML

[E04] 查找子串位置
来源：http://mobile.vehdjk.com/Article/details/gjhlkrauk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/goagjpgjm.sHtML


<!-- 参考信息 -->