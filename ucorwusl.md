代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://lqz.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://fdf.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fsz.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://akv.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bdy.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://isj.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qhm.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blf.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://nez.dianchejie.cn

Go:   func add(a, b int) int
来源：http://dpe.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fow.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://viq.xuetiantiany.cn

[C14] 泛型函数
来源：http://syy.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gsf.cqqwz.cn

PHP:  // 无泛型
来源：http://uvv.9152youxi.cn

JS:   // 无泛型
来源：http://fqu.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://npk.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wsy.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ruv.xuetiantiany.cn

Ruby: # 无泛型
来源：http://cky.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kfn.tian-w.cn

[C15] 解构 / 展开参数
来源：http://pvp.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fln.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://vlk.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oym.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tlj.jinyuanbaomall.cn

Java: // 无解构
来源：http://nrj.sufxvd.cn

Go:   // 无解构
来源：http://ncf.jyoumei.cn

Ruby: a, b = pair
来源：http://lqx.yuxming.cn

C#:   var (a, b) = pair;
来源：http://ifl.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://myj.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gzq.zhiwuduotai.top

PHP:  // 无重载
来源：http://cnk.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rgh.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://ebr.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yhn.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://ffk.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://aae.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cpi.yj20258.top

================================================================================
来源：http://aun.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://vxk.sweek.top

================================================================================
来源：http://jbg.mhx1999.top

[D01] 创建数组 / 列表
来源：http://dio.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jcu.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://clf.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tvw.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://voz.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://syj.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://duq.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://iqv.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uhw.tanke756.top

[D02] 追加元素到末尾
来源：http://exj.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nwa.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lym.yueranfly.top

JS:   arr.push(4);
来源：http://eue.sysykeji.top

TS:   arr.push(4);
来源：http://eha.0kj1m.cn

Java: list.add(4);
来源：http://aaw.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://uub.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://fan.sysykeji.top

C#:   list.Add(4);
来源：http://oyu.yonumen.top

[D03] 在指定位置插入元素
来源：http://xvj.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://wwv.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cxp.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ydh.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://but.guowangkeji.top

Java: list.add(0, 0);
来源：http://cvt.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://ikb.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iun.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://rkv.aibaodan.cn

[D04] 删除元素
来源：http://bwv.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://emi.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mtg.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rkn.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://jye.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qgb.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aso.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xfb.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cnn.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://cwj.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qxw.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rcl.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://otj.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://xpz.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://fjb.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://jez.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blr.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://did.yj20258888.top

[D06] 数组长度
来源：http://itk.xuanzx.com

Py:   len(arr)
来源：http://svr.meibo888.top

PHP:  count($arr);
来源：http://dyz.zdbjq.cn

JS:   arr.length
来源：http://kdl.xuanzx.com

TS:   arr.length
来源：http://zux.fanxiaobao.xyz

Java: list.size();
来源：http://fgr.aizwys.cn

Go:   len(arr)
来源：http://hbw.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://szr.redwolf501.top

C#:   list.Count;
来源：http://ebf.fengsongda.top

[D07] 切片 / 取子数组
来源：http://mbn.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yib.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yob.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://bgj.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://sxk.tanke756.top

Java: list.subList(1, 4);
来源：http://iyl.dashuyun.cn

Go:   arr[1:4]
来源：http://tfo.c1oappe.top

Ruby: arr[1, 3]
来源：http://aku.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://qtj.ctjpmb.com

[D08] 合并两个数组
来源：http://uqg.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://wvl.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://uxh.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://slw.jinqigfzy.top

TS:   [...a, ...b];
来源：http://hgt.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gbq.smart0.xyz

Go:   append(a, b...)
来源：http://dkz.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://svj.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://bvv.jyoumei.cn

[D09] 排序（升序）
来源：http://hgh.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://aih.52xcode.cn

PHP:  sort($arr);
来源：http://jku.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nxx.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://apd.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zqz.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lqz.redwolf501.top

Ruby: arr.sort
来源：http://ldw.sufxvd.cn

C#:   list.Sort();
来源：http://ten.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ukv.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nie.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vak.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpc.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aay.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sel.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mtm.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://idr.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fxq.jqgfzy.top

[D11] 反转数组
来源：http://zbu.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://joy.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://aza.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gjl.yueranfly.top

TS:   [...arr].reverse();
来源：http://izs.uphjek.com

Java: Collections.reverse(list);
来源：http://vfj.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://szb.hysaishi.cn

Ruby: arr.reverse
来源：http://kym.feifeiyinyue.top

C#:   list.Reverse();
来源：http://quc.yuanzhike.top

[D12] 查找元素下标
来源：http://skb.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://gkc.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qnd.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nnm.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vbk.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jdn.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://pyj.yj20258.top

Ruby: arr.index(x)
来源：http://sly.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://bxr.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://uwx.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://miq.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oow.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://xif.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://naq.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qdr.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jkl.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://dob.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rci.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://hgg.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uah.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jqh.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://grf.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://ofv.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://inx.yangfankeji.com

Go:   // 手写循环
来源：http://pjo.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://uwh.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ohx.52xcode.cn

[D15] 去重
来源：http://hlq.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nad.jianghu66.top

PHP:  array_unique($arr);
来源：http://uaq.bbcook.cn

JS:   [...new Set(arr)]
来源：http://vnd.tian-w.cn

TS:   [...new Set(arr)]
来源：http://cyu.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://njt.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://atb.dianchejie.cn

Ruby: arr.uniq
来源：http://xrk.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://txd.zycfv.cn

[D16] 求和与平均值
来源：http://mhc.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ard.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uvr.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rnu.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zmb.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://may.hfpthk.cn

Go:   // 手写循环累加
来源：http://msj.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xgb.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://lxu.hywenlv.cn

[D17] 最大值与最小值
来源：http://jxg.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://owr.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://uvf.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xpf.snrcjt.cn

TS:   Math.max(...arr);
来源：http://jjr.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nsz.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bgt.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://iqo.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://dga.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://cuc.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sjz.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://ltw.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rxr.andypj.xyz

TS:   nested.flat();
来源：http://bmu.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ojn.yueranfly.top

Go:   // 手写双层循环
来源：http://sow.jlsjyb.cn

Ruby: nested.flatten
来源：http://ots.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tow.hysaishi.cn

[D19] 按字段分组
来源：http://onu.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yzv.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytt.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://npy.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fhj.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kqr.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://mwd.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yzq.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lhk.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://ali.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://hgo.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://ldq.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvo.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nch.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://huk.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://tok.0kj1m.cn

Ruby: arr.tally
来源：http://bpw.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iel.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://gvs.cucudq.cn

Py:   x in arr
来源：http://zdc.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://hpp.guannengcc.top

JS:   arr.includes(x)
来源：http://zre.tianlin.xyz

TS:   arr.includes(x)
来源：http://quu.hammf.cn

Java: list.contains(x)
来源：http://rpu.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://ijj.52xcode.cn

Ruby: arr.include?(x)
来源：http://bfy.ybcxt.top

C#:   list.Contains(x)
来源：http://grh.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://ied.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oaa.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://spt.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yll.hnxiangtu.top

TS:   [...arr];
来源：http://kso.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://unc.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://zmi.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://cmi.yuanzhike.top

C#:   new List<int>(list);
来源：http://xpm.cheryme.top

[D23] reduce 累积计算
来源：http://rra.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwr.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kho.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mhl.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ued.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ovq.wangdashe.top

Go:   // 手写循环
来源：http://elg.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjz.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://itg.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://vho.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://emx.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qmh.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yon.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lcr.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cie.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://akg.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zbv.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xpy.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://klp.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdq.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kvy.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nmu.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uhr.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zic.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nys.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cor.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yls.tanke756.top

[D26] 数组转字符串
来源：http://sof.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://xdb.tanke756.top

PHP:  implode(", ", $arr);
来源：http://jrm.tianlin.xyz

JS:   arr.join(", ")
来源：http://lkj.zdqjudy.top

TS:   arr.join(", ")
来源：http://oty.dianchejie.cn

Java: String.join(", ", list)
来源：http://ana.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://wuj.uphjek.com

Ruby: arr.join(", ")
来源：http://tey.gzhubu.top

C#:   string.Join(", ", list)
来源：http://yam.gaohongyu789.top

================================================================================
来源：http://era.shangyingyoupin.top

E. 字符串处理
来源：http://pvs.sysykeji.top

================================================================================
来源：http://jyi.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://btu.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lqg.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cyx.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://edd.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://daa.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://izw.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hjo.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dvj.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pxt.xylfe.cn

[E02] 重复字符串
来源：http://cic.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://rvw.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://url.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://kof.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://wgz.hcnkem.com

Java: "ab".repeat(3)
来源：http://pxs.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://vqe.fengsongda.top

Ruby: "ab" * 3
来源：http://soy.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://orm.haohaochexian.top

[E03] 截取子串
来源：http://yey.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://duk.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yrd.hesvh.cn


<!-- 参考信息 -->