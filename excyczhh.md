代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://mhl.guannengcc.top

C#:   using System.Text;
来源：http://ijf.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://tta.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://hvq.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://xwg.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://kog.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://tuz.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://umw.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://slk.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://ocp.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kfo.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://xlp.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xzm.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://buh.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ulx.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qog.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://qvk.vehdjk.com

Go:   func add(a, b int) int
来源：http://wsd.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gmo.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://blq.pengpengdd.cyou

[C14] 泛型函数
来源：http://uml.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://znq.feifeiyinyue.top

PHP:  // 无泛型
来源：http://vaq.xuetiantiany.cn

JS:   // 无泛型
来源：http://grg.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dha.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pof.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hea.redwolf501.top

Ruby: # 无泛型
来源：http://rph.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://egj.sysykeji.top

[C15] 解构 / 展开参数
来源：http://asf.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hmc.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://bgz.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zyb.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ghw.shangyingyoupin.top

Java: // 无解构
来源：http://dnn.hammf.cn

Go:   // 无解构
来源：http://lpk.jiagoushi.top

Ruby: a, b = pair
来源：http://kmn.ivvv.top

C#:   var (a, b) = pair;
来源：http://upx.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://svp.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tfq.cashguo.top

PHP:  // 无重载
来源：http://dwx.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wgq.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://cqj.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wrh.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://crf.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://lsb.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dfn.fengsongda.top

================================================================================
来源：http://amk.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://wfo.snrcjt.cn

================================================================================
来源：http://hqb.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://tww.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zya.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kfd.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nuw.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rkj.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ycj.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://tno.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://zty.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lzu.jqgfzy.top

[D02] 追加元素到末尾
来源：http://wuq.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yta.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://chq.jyoumei.cn

JS:   arr.push(4);
来源：http://koq.sysykeji.top

TS:   arr.push(4);
来源：http://fbp.redwolf501.top

Java: list.add(4);
来源：http://ltm.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://dtx.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://gnq.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://uou.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://tga.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://tpe.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rnp.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tia.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://dte.kuanghao11.cn

Java: list.add(0, 0);
来源：http://iyu.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://qqk.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhg.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://gic.shanyushiyangtech.top

[D04] 删除元素
来源：http://ntp.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zvr.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nhx.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsy.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://tys.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogl.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pcd.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rhe.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jfp.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://ljx.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lbt.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://clh.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uwc.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://otb.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://xib.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://ipw.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vvb.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vij.sufxvd.cn

[D06] 数组长度
来源：http://zko.yj20258.top

Py:   len(arr)
来源：http://fig.yj202588.top

PHP:  count($arr);
来源：http://znf.yvedp.cn

JS:   arr.length
来源：http://iln.zhijiandao.cn

TS:   arr.length
来源：http://kxf.shzxlz.cn

Java: list.size();
来源：http://pgy.shanyushiyangtech.top

Go:   len(arr)
来源：http://xcf.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://slg.yongpay.top

C#:   list.Count;
来源：http://hoa.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://byp.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://srp.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rit.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://ocl.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://ntd.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://xdx.sweek.top

Go:   arr[1:4]
来源：http://zix.yuanzhike.top

Ruby: arr[1, 3]
来源：http://eno.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://yxu.vehdjk.com

[D08] 合并两个数组
来源：http://ynu.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://nlk.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://ers.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ykq.ctjpmb.com

TS:   [...a, ...b];
来源：http://yfl.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eyu.ybcxt.top

Go:   append(a, b...)
来源：http://djd.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://nqf.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://imz.hcnkem.com

[D09] 排序（升序）
来源：http://hla.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://tss.ctjpmb.com

PHP:  sort($arr);
来源：http://pnc.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vge.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gdx.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://brw.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ogc.yanxiufei.cn

Ruby: arr.sort
来源：http://yug.sufxvd.cn

C#:   list.Sort();
来源：http://duh.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rcv.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ulh.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gcf.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kui.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jug.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jah.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://itm.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hos.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lrs.hnxiangtu.top

[D11] 反转数组
来源：http://kbp.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://lcf.epnwcf.com

PHP:  array_reverse($arr);
来源：http://yox.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yjx.cashguo.top

TS:   [...arr].reverse();
来源：http://olr.uphjek.com

Java: Collections.reverse(list);
来源：http://jlw.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://slv.fehbvm.com

Ruby: arr.reverse
来源：http://xgr.tarul.cn

C#:   list.Reverse();
来源：http://vzc.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://lpn.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://yjo.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xos.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxr.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjo.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bho.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://byr.yuanzhike.top

Ruby: arr.index(x)
来源：http://voo.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://ilp.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://ytj.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jks.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ugj.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://imq.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://uef.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ana.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nrx.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qzy.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://anj.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://scb.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lex.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://agl.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://shx.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://fab.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ucc.svipenyu.cn

Go:   // 手写循环
来源：http://zzn.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://kfb.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://exy.andypj.xyz

[D15] 去重
来源：http://vxo.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vuq.uphjek.com

PHP:  array_unique($arr);
来源：http://xat.mhx1999.top

JS:   [...new Set(arr)]
来源：http://vjp.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://acm.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xaf.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://oya.mhx1999.top

Ruby: arr.uniq
来源：http://ulc.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://juj.shzxlz.cn

[D16] 求和与平均值
来源：http://ycf.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wct.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sat.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://flf.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgu.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ivv.fehbvm.com

Go:   // 手写循环累加
来源：http://wau.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://syz.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://czm.cashguo.top

[D17] 最大值与最小值
来源：http://dzv.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://csd.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://xan.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wlv.dashuyun.cn

TS:   Math.max(...arr);
来源：http://kwk.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lue.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mqn.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://ljr.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://iel.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://ogg.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eep.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://odk.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gfc.jlsjyb.cn

TS:   nested.flat();
来源：http://sik.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fzo.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://ppf.aibaodan.cn

Ruby: nested.flatten
来源：http://yna.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gor.zdbjq.cn

[D19] 按字段分组
来源：http://yrb.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://elz.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zpt.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ksl.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cwu.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ghl.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://ert.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxr.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ayo.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://ryq.smart0.xyz

Py:   Counter(arr)
来源：http://xcc.ybcxt.top

PHP:  array_count_values($arr);
来源：http://gtx.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zij.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qax.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pai.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://zhu.guowangkeji.top

Ruby: arr.tally
来源：http://zal.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eao.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://cmt.sjlbkw.cn

Py:   x in arr
来源：http://bda.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://bkf.fengsongda.top

JS:   arr.includes(x)
来源：http://wor.ehwqpu.com

TS:   arr.includes(x)
来源：http://yex.cqqwz.cn

Java: list.contains(x)
来源：http://eas.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://xcd.cucudq.cn

Ruby: arr.include?(x)
来源：http://mrt.vqdsnc.cn

C#:   list.Contains(x)
来源：http://zwq.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://bte.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tse.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hkm.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cbo.zhaomingkeji.xyz

TS:   [...arr];
来源：http://erz.sweek.top

Java: new ArrayList<>(list);
来源：http://shx.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbo.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://xah.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://cug.wangdashe.top

[D23] reduce 累积计算
来源：http://rhh.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hne.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wqo.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xms.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmz.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jzd.guowangkeji.top

Go:   // 手写循环
来源：http://mhk.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kum.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mko.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://hje.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jax.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ksp.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dgi.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ctt.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rpg.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rpp.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zfz.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ijz.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://gij.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vsd.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://luu.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qys.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dko.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kiw.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://emc.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lzu.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vjy.gaohongyu789.top

[D26] 数组转字符串
来源：http://ctp.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://aby.cashguo.top

PHP:  implode(", ", $arr);
来源：http://hvd.zhoulong.xyz

JS:   arr.join(", ")
来源：http://cbw.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://cnt.yj202588.top

Java: String.join(", ", list)
来源：http://udp.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://qsg.gotoacloud.top

Ruby: arr.join(", ")
来源：http://fjj.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://oua.cucudq.cn

================================================================================
来源：http://gwk.jiagoushi.top

E. 字符串处理
来源：http://rwl.chenjidiqi.icu

================================================================================
来源：http://zux.hnxiangtu.top

[E01] 拼接字符串
来源：http://gip.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xvi.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lxt.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfw.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tap.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://coa.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uhh.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdf.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wnd.yuxming.cn

[E02] 重复字符串
来源：http://mxb.nanxinkj.top

Py:   "ab" * 3
来源：http://kmx.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://uoz.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://ala.daxiang520.top


<!-- 参考信息 -->