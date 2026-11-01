代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.yfazqb.com/Article/details/gsbilqesa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gkoihwmii.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gkdgtkthm.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/glpwpitev.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gxtavficj.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gljafyknf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gzhmwwmyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gizdzmnbq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwgpnumfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/gwkcgaroj.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjsnczuz.sHtML

Go:   // 无解构
来源：http://www.share.vehdjk.com/Article/details/gxtjtuzak.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/gkgnvwdhk.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gqkyjncfj.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gepcubzte.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gvumsxqql.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gfgvxnvsm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/gmjunmjgf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.sjlbkw.cn/Article/details/gdmlsbsuk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gfamgyitu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gkmycpgqv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gwjyaqkjq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gqgiezkbu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvmgeswmg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/geemojrdl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gosdmxgwd.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/geugdypds.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gwmnbksqs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gtvlihisr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvwubsgs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gjgvukgvv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gcmybnofn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.vehdjk.com/Article/details/ghaodgqsf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/ggifjszik.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gczuyneyu.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gsevqoiim.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gbzanlvev.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gvwrqfmxu.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gtvkeclgg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gxhasmymz.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/gwhxwirrm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gxmuhndyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gqycwchfl.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gyqtzqzfp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/grfiecndq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gyfwtqbym.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/ggolycamh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/gcfazsxdr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gnzhqhzhf.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gywedmhbb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/ggdhzdjnu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/ggluelltl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gwsackeal.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gatxzzrzc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/ghkjwphos.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gaumiimun.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gidboptcx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gdsfiwhmd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gcnspmgsv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/gqhouuvei.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gmjduikyq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gslghvnep.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gspovexbj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gozijbmrl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gtavwzcov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gfcpzrtfu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gmavmjhqb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gxonapmoy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gusqgkygk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gufhubcbj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gajvntoyl.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gumlknles.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gjixtcsal.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gnlijrtxc.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gwyoryasc.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gpblsgcxs.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/ghzgrbzhg.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gtlsrnkwq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/gqpgztlok.sHtML

C#:   list.Count;
来源：http://wap.vehdjk.com/Article/details/gbhntiyko.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gehlearew.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gncrzgpzq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gssymrivp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gqegwkehk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gbbroaifx.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gogowjdwu.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/gsgbnazwx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gyeayizau.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gnxxsuyyj.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gqylgfehf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gxotmfgps.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.vehdjk.com/Article/details/giqzbtrnx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fktsv.cn/Article/details/gpjeysrtl.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gfhbekzkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/ghzudhxkc.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/grsdjlcld.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gxyokwkxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gfwbuxvqj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyebqqox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gfxaqwjud.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/ggojrdahu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/gfqdgeyah.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/gyuzorobn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/gzaqmuymw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/glzdiovin.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/grmbyrvql.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gwfycpktl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gbplbzboa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gqtchaorp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gmtzyhbpi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhccducn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gnkltykso.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/gtfqnxffl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/gzloivrxp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gjwglhbxo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.yfazqb.com/Article/details/gueawqbdy.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gtvcrhzug.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gkrbzjqcx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gvzaqkbbz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/ggilvzftx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/goonwoplu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.bbcook.cn/Article/details/glwhrwwrz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gvclymids.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gkuqcuyjz.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gblslneht.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/gsldiymuh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/goyipotnm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gidbvgtia.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxseriezo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ghngkqolk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gwfmkwcig.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gilrkvlug.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gkabwzhip.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gdndxrihb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gozjxkaua.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gjiqjieth.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gepteyqim.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gkgdthsxu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gsmustizh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gfpdrodhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gqvevucul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.yfazqb.com/Article/details/gdboaigut.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/ghfictwto.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gxaxqhmpl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gecilqphq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gubyitucw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gzeqwmovt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/grmziokny.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/gwxvoofct.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gaermusqr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gugjpaliw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gqwqflonc.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gxtazlqty.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gtudfbvms.sHtML

PHP:  array_unique($arr);
来源：http://wap.fktsv.cn/Article/details/gomuerjqq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/guwvpnzuq.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/glrhcxdzm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gploenxgl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gmipminle.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gzbnamflq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/glpqkbecj.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gtsqgyxwv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/guzcighrv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gymltvioq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gltgwbqdq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbadhbblj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gfgrkqton.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/ghxkhaweu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gluuwflbs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gktbrtngu.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gumefqxog.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/giyydtdxh.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gdlqwikxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gsyatxjbc.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gebvcodln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gxyrhjvzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gymudsuze.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gagvtozqk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gomxibjya.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/gtzkciwsi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gwcefbnvb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/grihqgofv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gklhfhgea.sHtML

TS:   nested.flat();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjxbhftr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfzdjzpjl.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gdrnnldrr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/glvvzibgi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/grjwpiaps.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gyriwqymt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gzhmebgbn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gctyfqjzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gcyljvnzo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gbykomkui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gzqelnbjn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gmneaxpvo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gvkpwbqlu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gmiejwaoz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gahtcrdrh.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gmlwrhxta.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzpmxzluj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gjwgcsvfz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gnnwahpav.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/giyomfqfp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gtjrbbrkl.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gihnrfvbn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gjgshpidd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/giuzhjbms.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gmbegbvap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gzqpfxeej.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gbrleqalm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gleltxbkd.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gtvkonnam.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gyqttnble.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gavpyfccx.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gdjcmxgei.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/gjqoiwenq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/ggvlibbra.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gdqaryynf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkecdzolj.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/ggdwfgggo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gmnamcygz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gsalaaeoh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gmytwieoc.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gyylqzegi.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/goeqoxojd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gcovlwyhf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/guulaaqhl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gbafcmaln.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gvzxwjvbn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/galrgccbn.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gjnunschk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gqopmecpe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.vehdjk.com/Article/details/gkdiyjead.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/ggjjsuhks.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gozqawjso.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/gijwrxrjz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gdjbubfdl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gyltjeiko.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gxvlawmwa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gyptlkxup.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gpdqganhc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbrbumyq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/guinxgqmn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/glhtyfqtq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/giituekvw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gqyvpzwya.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gaijjswki.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gsasdhswi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gefyhxqat.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbavtgbfl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gwamogzql.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gkldqizme.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.vehdjk.com/Article/details/gyxmiyomu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gogpevoon.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/ghsowurud.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/goirtfdwg.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gnonsyuqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gptuvuflf.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gscpsgame.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gzhbohfzc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gaqlmfsgo.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gwvfhjwpj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gosahsefu.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/geqvjlput.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gtzndwrfs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gdjwpyoeg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gtuqfcker.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gvwivazoh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/ghiejxblz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gisooirtj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gfmdxloix.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gjciiylwv.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gxstcuhyd.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gtvckzupj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/gncwnvdld.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gqkydejqg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gpcghnahf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/ggpitqiaa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gsiobjlrn.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/ghynjqfzv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gjvsmxuus.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gaawwqmyo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gzieaospr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gjykemsoh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gobcmavdv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gvjfscdcf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gfibcthyj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gdyfldoiq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gzckjregc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/ghkxlpqea.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/gzxwmqpzj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gxdrtpwrw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gunzokhrf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gdctlyeku.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gccarrvgz.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gyezwitpn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gtonywgwx.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gtxowbecb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/ghgwvmuoh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gtlktiyfi.sHtML


<!-- 参考信息 -->