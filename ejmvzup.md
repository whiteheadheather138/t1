代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gwsvmasbb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gwgqfjqzf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/ggfibcbjk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gdodncpnv.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gtuquuzmi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/gbftzmpib.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gurbdwdic.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gahyprkbx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/gonsjdtwy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gsekvxhkx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gkzlmsgpd.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gwxylgrfa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fktsv.cn/Article/details/gtzwrbibx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/gedscofrm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/gyyneshqf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/gmmgtpgro.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gpdxehqew.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fktsv.cn/Article/details/gvrwkrwfj.sHtML

Java: // 无解构
来源：http://www.share.yfazqb.com/Article/details/gyeihbrcg.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gvbxptpit.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gyijxaroy.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gylzkvjyc.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/giytwbjxo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gpdptthag.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gtjozclmc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gxoipvldl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gjexstkxu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gpmfkwmcc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gojxihugh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gjucvkbud.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gxbygvsfc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gexbaopjy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gnhlpjsbh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gefucsegr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gjusdzrzd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/glylcnxjc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/ghkdkubin.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gbvmrqljw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/ggffnsvgx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gjkpskvbr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gzjxgiznx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gicbprtrd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gilclxbyd.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gpbypzhye.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gzohrdxtd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gqkhhpqih.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gychgpfry.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gqubrmnll.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gwxybwwqw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gqqtbavgh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/gzuvbbptj.sHtML

C#:   list.Add(4);
来源：http://wap.epnwcf.com/Article/details/gebxgoomo.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gqiavadyw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/gxcnlmwer.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gfiyhqzsv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gjxrdkmqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gauvuxdfw.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gvjtzpvgw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.epnwcf.com/Article/details/gpycdqclr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/gfcrgdrzl.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gzjbbggpl.sHtML

[D04] 删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gvstdcqnb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gyyxnjtcc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/grwoiywqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gdihuxuhv.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gvvlrpisd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gecdvdyhq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gxeqvnmec.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/guqjshiaa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gycpekcsb.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gvlaunsau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gnbqujjov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gglpgjaow.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gyienmsyb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gsivcceqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/gbrfamimx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gjrkbjtqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/groeltjwh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gdihpaxxz.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gxljfkisu.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gohwazqst.sHtML

PHP:  count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glnsjnlpn.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/glhwckqtg.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/giaogvrmk.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gocpsaqhx.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbluqbiav.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/gsqknnwcv.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gpywghedh.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gekadutqx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gwzocduoh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gcpwkitar.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/grtuovzps.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gnfenxqjq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gfplfvbrv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gadwxsihl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/gwmmgfehq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/gqsqkvjic.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/goomlqscd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/grtcaionk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gjwwxtfng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gjngcjxgx.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/goozbnqln.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.sjlbkw.cn/Article/details/gzfuzobps.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gbfuswonk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gvkmzineh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gqwxnegvy.sHtML

[D09] 排序（升序）
来源：http://www.m.share.vehdjk.com/Article/details/grkcqhhkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gorrjhdxu.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gjtosxarx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.bbcook.cn/Article/details/gxpenqrak.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gycryudhr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gnnkshwqf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gimjvhwhf.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gdoalfvzq.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gtomzdwrb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gnfynmxvi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/giljuiipt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gfftovlex.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/grzsposbd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gtyftyiau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gbivbyzbh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gmkaaygwc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/ggopqbcjf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gmovltryd.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gnvppkqhu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gepvejpfc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/grtycobhs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gpnoxqmtd.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gwhepeydd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/grbozulwr.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gllkhlbth.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gmdjbfulx.sHtML

C#:   list.Reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gcuazfjkw.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gurnmxwer.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gggzzftjx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gkutffdgr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gecjdfrot.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gishakdlt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/giyudmtqs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ggvtpihoy.sHtML

Ruby: arr.index(x)
来源：http://www.share.tarul.cn/Article/details/ghzykvngq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.vehdjk.com/Article/details/glqftjjyg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/goxhgfuuz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/gtnueqlne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gwabcudxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gndpzhrbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gzdiiqrkq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gwjttsslc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/grzslumks.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gtzoehqfs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gbuedhkxg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gzquigsyh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gncvhrozs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/goaalxnna.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gnhbszkpj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gpozuyabp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.epnwcf.com/Article/details/gwdgkhnsm.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/guvfujjvv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gctccizmr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gimnocqbg.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gtbmmyflb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gbbtxxjkw.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gwuabipzn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/glanbjpqf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gglupqpsx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/ggfqsqdku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gkctbdtmu.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gytevdaot.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/gwtzodxgh.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/gjusfdcyz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gqxjsrkbd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gbsdhjauh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gacodfsjp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gxvnmbltf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gbivjgdoe.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gqbwrniyl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/glstwgelc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gibjjkjlc.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gkrxogwvb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gdasrsjqx.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gyhsscslw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gaphdtijd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gakforiuj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gnfzlcqne.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gxomcifzi.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gltylrnif.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/glfmrbppv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gwqibojib.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/ggrctuxtz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/givzhuzzj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/gquyticya.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gifwotafv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/givdaoexj.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gzjodvypf.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/guuccedwx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/grxouywxw.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gvkcstmvx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gatdpltze.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/grunuhgeo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gwxxuszzy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/giqzbelph.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gxihsmzjz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/goosleyzm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gawkkmzuh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/gajibjmez.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gzhnauhci.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gtvwutxzs.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glluaydyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/guchvrfku.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gkeoizmni.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/gzxmetzsj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gnkwpxaxl.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/gjqvhcuyy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gjajbiupi.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gkpdykdui.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/geeorggrn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gpmohyyip.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gnysmvjvn.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/glzlppaya.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gxtrebyns.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/geblvwkxr.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gjnsdvbeo.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gxyaymtjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/giohoqzki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gyjsceiil.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gfgubwffd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gprwuknrv.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gwessmrdl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gqibsutfj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/guxuozuxz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gdlvsqmqw.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gnnwgkapu.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gbzoebtpi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gagtvwuza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gvlmrxepl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gyqytbdzt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gtlivjwsa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/grhehsdxt.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gebtctpfv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gkmcrcsnm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/glompcnvj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/glluqjlxg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gcstzzobx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gyouffqze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gfvicsdst.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/gqsiqlwbs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkbxfija.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gzkzfuvha.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gxwuqlegr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gdeztofvz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gpfnocjpe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gasyieuyq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gibxcyfpb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/glavpktse.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gshedaoph.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/guvjszvmg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gwtanolsv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gguloqfdl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/ghrwzvbbt.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gvfdsfrnw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.bbcook.cn/Article/details/gzjicuslz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gqlehawio.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gewkpqpiq.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gznsfdiuw.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gihucredl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/gapivkewg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gvdbyszeq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gskjappur.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmfcswplk.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gwwyrluuq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzwdcnqxv.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gcyvdityt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gpnyziwwf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gqhqptvwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gsychhaoc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/ghdxramsi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gbwvfpxrj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fktsv.cn/Article/details/gxibxmkpq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gfytvactk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/gsaewtcny.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/glpqcbcpm.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gehpmrmnu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gcjuloqna.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjshzcgxb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/goufferau.sHtML

Java: "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gqgmnqvku.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gduidyjfz.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/guuetbcyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gixsjesxm.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/ggfmejxje.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gwbjmaggr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gsdoyyxrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/ghmtymgwk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gdfeowrdr.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gwmveulpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/ggfrkkdwy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gvejikjqp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/gzzgskwli.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gbrpopici.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/ggefybqxy.sHtML


<!-- 参考信息 -->