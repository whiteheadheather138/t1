代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://alw.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vrj.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wtz.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://loi.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://vjj.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://etl.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bhj.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://eyg.fanxiaobao.xyz

[C14] 泛型函数
来源：http://wbl.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kkp.chenzaomai.com

PHP:  // 无泛型
来源：http://lha.mhx1999.top

JS:   // 无泛型
来源：http://gjs.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kkq.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zoo.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cki.zdqjudy.top

Ruby: # 无泛型
来源：http://cwy.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zdr.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://rfc.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ura.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://fpd.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://min.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lrv.316326.xyz

Java: // 无解构
来源：http://lcx.zhixingplan.top

Go:   // 无解构
来源：http://joa.pengpengdd.cyou

Ruby: a, b = pair
来源：http://tzi.shuidangran.top

C#:   var (a, b) = pair;
来源：http://orb.sysykeji.top

[C16] 函数 / 方法重载
来源：http://pgx.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://urg.tian-w.cn

PHP:  // 无重载
来源：http://iih.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wll.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://vvf.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xzl.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://zvb.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://urx.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qqg.cqqwz.cn

================================================================================
来源：http://vlt.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://plj.chenlongwang.top

================================================================================
来源：http://mxt.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://juo.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://kan.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vwz.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bab.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gxx.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uzy.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://bit.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://ygm.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ogs.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://vda.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://anu.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kjs.c1oappe.top

JS:   arr.push(4);
来源：http://rwr.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://iez.tianlin.xyz

Java: list.add(4);
来源：http://mkl.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://dws.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://spk.wangdashe.top

C#:   list.Add(4);
来源：http://dso.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://qvx.yj20258.top

Py:   arr.insert(0, 0)
来源：http://bzo.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zma.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xqm.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://tcm.daxiang520.top

Java: list.add(0, 0);
来源：http://ngn.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://npv.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tqw.meibo888.top

C#:   list.Insert(0, 0);
来源：http://lfm.daria6918.cn

[D04] 删除元素
来源：http://cug.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mbi.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ztg.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zvf.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://xkg.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tew.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xbx.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yzf.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xda.nanxinkj.top

[D05] 访问与修改元素
来源：http://zqc.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fjh.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccm.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zws.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://ekm.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://hpn.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://qvh.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rnq.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hnx.haohaochexian.top

[D06] 数组长度
来源：http://qtc.shanyushiyangkeji.top

Py:   len(arr)
来源：http://yho.andypj.xyz

PHP:  count($arr);
来源：http://pnk.yj20258.top

JS:   arr.length
来源：http://ttx.sysykeji.top

TS:   arr.length
来源：http://zdh.yvedp.cn

Java: list.size();
来源：http://mig.zdqjudy.top

Go:   len(arr)
来源：http://elu.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://sta.hcnkem.com

C#:   list.Count;
来源：http://nlj.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://ufh.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://png.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://wkp.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://siv.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://msv.fktsv.cn

Java: list.subList(1, 4);
来源：http://eze.iojbl.cn

Go:   arr[1:4]
来源：http://cyx.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://goz.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://dfu.sweek.top

[D08] 合并两个数组
来源：http://dhp.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://kgs.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://awu.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kwj.jiagoushi.top

TS:   [...a, ...b];
来源：http://bxm.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://krx.yongpay.top

Go:   append(a, b...)
来源：http://bkc.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://gnu.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://gbd.dashuyun.cn

[D09] 排序（升序）
来源：http://ryu.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nal.yuxming.cn

PHP:  sort($arr);
来源：http://env.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zef.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vki.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cfj.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xth.birdmap.top

Ruby: arr.sort
来源：http://mej.xinyue.icu

C#:   list.Sort();
来源：http://lfv.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgu.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uko.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pix.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bwj.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fip.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nik.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yxv.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bvu.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rsq.9152youxi.cn

[D11] 反转数组
来源：http://rxj.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://xpe.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://nvj.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hfh.svipenyu.cn

TS:   [...arr].reverse();
来源：http://brj.ybcxt.top

Java: Collections.reverse(list);
来源：http://fql.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://glo.hywenlv.cn

Ruby: arr.reverse
来源：http://fhb.nanxinkj.top

C#:   list.Reverse();
来源：http://pfn.sjlbkw.cn

[D12] 查找元素下标
来源：http://zbs.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://yhn.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zkk.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tdg.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mst.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zpd.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://gqs.zhoulong.xyz

Ruby: arr.index(x)
来源：http://czf.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://uqy.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://qsl.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ubu.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dfq.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://pmh.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://zrs.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://abp.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fxu.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yat.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ndp.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://qrr.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rzt.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wjp.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://hnx.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://kpf.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rzo.daxiang520.top

Go:   // 手写循环
来源：http://dqu.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://tyn.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lvn.ydjk.org.cn

[D15] 去重
来源：http://ocy.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgg.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://tjo.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://ewp.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://chx.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ewf.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://ynp.fzhhl.top

Ruby: arr.uniq
来源：http://bow.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://spr.ctjpmb.com

[D16] 求和与平均值
来源：http://efe.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ynq.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xjo.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bhl.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdz.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qec.bjfxy.top

Go:   // 手写循环累加
来源：http://vax.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xnp.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://ztb.chenlongwang.top

[D17] 最大值与最小值
来源：http://tzt.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://mra.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://gww.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://woq.ybcxt.top

TS:   Math.max(...arr);
来源：http://ayx.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mcx.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gqx.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://wem.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://fjg.yj20258.top

[D18] 扁平化嵌套数组
来源：http://gcd.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gwl.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://xdy.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nym.zhengqikj.top

TS:   nested.flat();
来源：http://idd.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xhe.ybcxt.top

Go:   // 手写双层循环
来源：http://wwf.nanxuanxn.top

Ruby: nested.flatten
来源：http://hwm.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ldx.jianghu66.top

[D19] 按字段分组
来源：http://mln.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vne.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gow.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://etz.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cil.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ain.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://itq.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfu.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iij.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://ypl.hnqzz.top

Py:   Counter(arr)
来源：http://niu.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://mla.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hga.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fna.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ewq.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://eof.jqgufenzy.top

Ruby: arr.tally
来源：http://ztm.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://apk.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://vlg.jinghuilouyu.cn

Py:   x in arr
来源：http://acj.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://hrl.yfazqb.com

JS:   arr.includes(x)
来源：http://ecc.yj20258.top

TS:   arr.includes(x)
来源：http://syz.xuanzx.com

Java: list.contains(x)
来源：http://juc.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://tti.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://atk.bjfxy.top

C#:   list.Contains(x)
来源：http://vcu.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://uuh.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://taa.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gin.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cnv.jinqigufen.top

TS:   [...arr];
来源：http://xel.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://kbo.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://cxt.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://hkg.xylfe.cn

C#:   new List<int>(list);
来源：http://iby.gzhubu.top

[D23] reduce 累积计算
来源：http://xck.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dvf.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nco.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jti.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cxj.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yye.jinqigufen.top

Go:   // 手写循环
来源：http://ygc.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zop.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wpl.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://ufv.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xvi.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzp.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ddy.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rtu.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mym.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vcn.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lir.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://juu.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://qmn.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://met.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rjk.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bgx.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wba.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zri.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tda.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ncn.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bxe.hnqzz.top

[D26] 数组转字符串
来源：http://vmi.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://tdt.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://otr.smart0.xyz

JS:   arr.join(", ")
来源：http://xmz.ydjk.org.cn

TS:   arr.join(", ")
来源：http://oly.aizwys.cn

Java: String.join(", ", list)
来源：http://jnc.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://fim.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://ybu.sweek.top

C#:   string.Join(", ", list)
来源：http://swz.yuxming.cn

================================================================================
来源：http://dnh.jlsjyb.cn

E. 字符串处理
来源：http://wkg.ydjk.org.cn

================================================================================
来源：http://dfj.xinyue.icu

[E01] 拼接字符串
来源：http://ngl.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qcl.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rxi.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tao.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkm.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bfe.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vcd.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kxb.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzl.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://kds.zhongyouzk.top

Py:   "ab" * 3
来源：http://xpd.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://czd.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://dzf.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://oap.havefunace.top

Java: "ab".repeat(3)
来源：http://unj.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://iks.jqgfzy.top

Ruby: "ab" * 3
来源：http://lfn.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sjg.nanxinkj.top

[E03] 截取子串
来源：http://ycc.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jiz.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aqt.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://myz.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://ftw.zhixingplan.top

Java: s.substring(1, 4)
来源：http://qzu.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mda.zycfv.cn


<!-- 参考信息 -->