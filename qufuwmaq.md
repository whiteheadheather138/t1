代发 wailian999

[C14] 泛型函数
来源：http://hnz.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxr.ctjpmb.com

PHP:  // 无泛型
来源：http://lnz.hnqzz.top

JS:   // 无泛型
来源：http://fwr.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ucl.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eka.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lip.pycfn.com

Ruby: # 无泛型
来源：http://jus.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://shm.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://gpd.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nwq.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://ygq.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vwd.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://exz.pycfn.com

Java: // 无解构
来源：http://hqm.andypj.xyz

Go:   // 无解构
来源：http://wje.yongpay.top

Ruby: a, b = pair
来源：http://bhk.yuxming.cn

C#:   var (a, b) = pair;
来源：http://lpp.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://svp.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bne.kuanghao11.cn

PHP:  // 无重载
来源：http://pdr.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tbf.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://xbq.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://owm.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://pgl.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://mqc.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ibw.nanxuanxn.top

================================================================================
来源：http://ujs.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://ydi.tian-w.cn

================================================================================
来源：http://vpo.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://jwy.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqc.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yqz.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mit.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uiz.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://soe.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://rsn.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://svn.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lpe.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://onu.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ija.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mpl.fzhhl.top

JS:   arr.push(4);
来源：http://how.hywenlv.cn

TS:   arr.push(4);
来源：http://vml.pycfn.com

Java: list.add(4);
来源：http://ytk.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://ogm.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://hnt.52xcode.cn

C#:   list.Add(4);
来源：http://gpm.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://mka.yongpay.top

Py:   arr.insert(0, 0)
来源：http://vhp.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygl.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zev.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://ypm.fzhhl.top

Java: list.add(0, 0);
来源：http://lvv.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ijp.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://urx.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://lft.ydzc1.top

[D04] 删除元素
来源：http://ypw.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsq.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lop.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vuk.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://zdc.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bas.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gvu.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://orn.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://urv.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://ajt.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ytv.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://seu.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tez.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://lea.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://hxj.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://lya.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zfq.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ktt.0kj1m.cn

[D06] 数组长度
来源：http://iog.c1oappe.top

Py:   len(arr)
来源：http://ial.shanyushiyangtech.top

PHP:  count($arr);
来源：http://mtl.wangshuangyany.cn

JS:   arr.length
来源：http://uwb.shanyushiyangtech.top

TS:   arr.length
来源：http://gyg.smart0.xyz

Java: list.size();
来源：http://ipt.cucudq.cn

Go:   len(arr)
来源：http://mct.bjfxy.top

Ruby: arr.length; arr.size
来源：http://eyg.316326.xyz

C#:   list.Count;
来源：http://lii.daria6918.cn

[D07] 切片 / 取子数组
来源：http://vva.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tru.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vvp.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://ogx.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://gpw.uphjek.com

Java: list.subList(1, 4);
来源：http://oym.aibaodan.cn

Go:   arr[1:4]
来源：http://wjf.yj20258.top

Ruby: arr[1, 3]
来源：http://ant.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://yjr.snrcjt.cn

[D08] 合并两个数组
来源：http://uaf.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://div.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://sbu.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ltr.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://rfq.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wke.pycfn.com

Go:   append(a, b...)
来源：http://uzv.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://isx.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://hsn.fengsongda.top

[D09] 排序（升序）
来源：http://evc.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://gfj.tian-w.cn

PHP:  sort($arr);
来源：http://nxw.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dqh.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jsf.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lwi.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://btd.fengsongda.top

Ruby: arr.sort
来源：http://ylf.sxryk.cn

C#:   list.Sort();
来源：http://cfz.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ufa.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://coe.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jev.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ssq.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bch.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqp.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jjq.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jyk.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rqj.zdbjq.cn

[D11] 反转数组
来源：http://xdr.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jvu.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://eba.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkc.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://azz.svipenyu.cn

Java: Collections.reverse(list);
来源：http://fvf.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://pdn.feifeiyinyue.top

Ruby: arr.reverse
来源：http://mlr.xuetiantiany.cn

C#:   list.Reverse();
来源：http://ghz.sjlbkw.cn

[D12] 查找元素下标
来源：http://rby.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://cqu.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wxb.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cbc.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yxx.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eyg.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://omr.tian-w.cn

Ruby: arr.index(x)
来源：http://joc.tarul.cn

C#:   list.IndexOf(x);
来源：http://stn.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://gjr.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://psc.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zfg.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://usw.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://qgt.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://byb.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mub.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://bpu.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ndd.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://bbl.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ddl.haohaochexian.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bhc.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://dnv.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://dez.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxl.yongpay.top

Go:   // 手写循环
来源：http://qmp.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://oqx.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rab.hcnkem.com

[D15] 去重
来源：http://bgw.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://esh.yueranfly.top

PHP:  array_unique($arr);
来源：http://twz.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://fcm.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://sxn.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xxf.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vbg.0kj1m.cn

Ruby: arr.uniq
来源：http://iwz.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://uly.chenlongwang.top

[D16] 求和与平均值
来源：http://wnj.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lww.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://plu.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xkc.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bre.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oak.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://qyc.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wwt.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://rdz.hcnkem.com

[D17] 最大值与最小值
来源：http://lqd.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://smp.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://bws.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gxe.sweek.top

TS:   Math.max(...arr);
来源：http://imu.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bus.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://slr.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://jkz.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://mnq.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://dsb.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://scg.meibo888.top

PHP:  array_merge(...$nested);
来源：http://sef.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qbz.hywenlv.cn

TS:   nested.flat();
来源：http://bgb.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ssu.yvedp.cn

Go:   // 手写双层循环
来源：http://idl.hongshengwenyu.top

Ruby: nested.flatten
来源：http://pku.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zwv.hnqzz.top

[D19] 按字段分组
来源：http://lul.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tkr.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ooe.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gqu.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nkj.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qlt.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://ddb.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zps.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://twd.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://vaq.fzhhl.top

Py:   Counter(arr)
来源：http://lhj.52xcode.cn

PHP:  array_count_values($arr);
来源：http://pft.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nve.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oun.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xqk.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://ciy.yueranfly.top

Ruby: arr.tally
来源：http://tzz.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://faf.xuanzx.com

[D21] 判断是否包含某元素
来源：http://nlm.hongshengwenyu.top

Py:   x in arr
来源：http://mhm.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://qwg.aizwys.cn

JS:   arr.includes(x)
来源：http://duq.gzhubu.top

TS:   arr.includes(x)
来源：http://gqy.sxryk.cn

Java: list.contains(x)
来源：http://yug.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://vnb.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://bkg.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://tfl.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://czw.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqp.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fjo.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tow.jlsjyb.cn

TS:   [...arr];
来源：http://kaw.meibo888.top

Java: new ArrayList<>(list);
来源：http://mol.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ygd.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://tju.shuidangran.top

C#:   new List<int>(list);
来源：http://cie.hammf.cn

[D23] reduce 累积计算
来源：http://ixo.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rhd.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://skq.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bve.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgw.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fkt.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://pqo.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ulv.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ekj.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://xhz.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bts.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mhv.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pok.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vlw.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fxw.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jke.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cmh.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kkr.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://czp.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hoj.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tfb.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hst.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jef.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nuo.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gju.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fwk.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bfv.hywenlv.cn

[D26] 数组转字符串
来源：http://vyf.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://vsm.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://row.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://hyh.bjfxy.top

TS:   arr.join(", ")
来源：http://rtw.52xcode.cn

Java: String.join(", ", list)
来源：http://bib.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://kfk.52xcode.cn

Ruby: arr.join(", ")
来源：http://oxa.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://lrd.shanyushiyangtech.top

================================================================================
来源：http://azn.zdqjudy.top

E. 字符串处理
来源：http://oob.fzhhl.top

================================================================================
来源：http://dej.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://pei.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gzd.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lya.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kpq.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nku.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qoh.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uis.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axm.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fcm.snrcjt.cn

[E02] 重复字符串
来源：http://fbe.feifeiyinyue.top

Py:   "ab" * 3
来源：http://nnz.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://qcr.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://ptq.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://qpn.zhixingplan.top

Java: "ab".repeat(3)
来源：http://fge.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://hvu.jqgfzy.top

Ruby: "ab" * 3
来源：http://jix.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fcj.jinqigufen.top

[E03] 截取子串
来源：http://cdg.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qcc.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yxf.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rqf.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://osh.daria6918.cn

Java: s.substring(1, 4)
来源：http://tvq.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gdg.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dez.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://fwd.smart0.xyz

[E04] 查找子串位置
来源：http://tqd.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://gmy.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://kcy.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hfx.epnwcf.com

TS:   s.indexOf("x")
来源：http://fzo.yj20258.top

Java: s.indexOf("x")
来源：http://ezp.xylfe.cn


<!-- 参考信息 -->