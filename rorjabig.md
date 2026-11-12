代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://olb.birdmap.top

C#:   using System.Text;
来源：http://edk.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://csi.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://tjn.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://fuz.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://blu.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://fxt.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ale.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://fnx.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://zcp.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://smr.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://rlj.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xyb.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dje.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umr.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kli.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://app.fktsv.cn

Go:   func add(a, b int) int
来源：http://sis.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rfp.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://gsy.xinyue.icu

[C14] 泛型函数
来源：http://zbd.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dlm.smart0.xyz

PHP:  // 无泛型
来源：http://fuh.ivvv.top

JS:   // 无泛型
来源：http://gqu.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hia.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://czw.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dlx.zhijiandao.cn

Ruby: # 无泛型
来源：http://saf.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://buj.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://vru.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ahm.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ehf.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pam.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dlq.yvedp.cn

Java: // 无解构
来源：http://ijw.shangyingyoupin.top

Go:   // 无解构
来源：http://qlb.xuanzx.com

Ruby: a, b = pair
来源：http://irf.zycfv.cn

C#:   var (a, b) = pair;
来源：http://zoe.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://ccs.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qbl.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://ocw.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://szn.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://qxq.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dhi.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://bau.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://mgg.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://puk.shuidangran.top

================================================================================
来源：http://sqg.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://qku.tanke756.top

================================================================================
来源：http://gcs.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://jgv.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://btm.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ctn.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ojr.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zan.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rjm.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://fvl.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://git.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uly.fktsv.cn

[D02] 追加元素到末尾
来源：http://opo.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://niy.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fyj.ivvv.top

JS:   arr.push(4);
来源：http://tyr.aibaodan.cn

TS:   arr.push(4);
来源：http://dvm.ydjk.org.cn

Java: list.add(4);
来源：http://fcr.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://mgx.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://pdt.vehdjk.com

C#:   list.Add(4);
来源：http://vme.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://zvh.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://olv.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vkh.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jlz.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://mcu.nanxinkj.top

Java: list.add(0, 0);
来源：http://xra.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nzq.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ugl.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://cov.ivvv.top

[D04] 删除元素
来源：http://esc.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dwj.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lnf.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yqp.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://rix.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gbd.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rga.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tzb.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pee.hfpthk.cn

[D05] 访问与修改元素
来源：http://nqs.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpw.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ovh.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://idb.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://frb.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://bwe.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://zvk.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xqa.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lrl.ydjk.org.cn

[D06] 数组长度
来源：http://zjc.shanyushiyangtech.top

Py:   len(arr)
来源：http://iue.sjlbkw.cn

PHP:  count($arr);
来源：http://ixf.fzhhl.top

JS:   arr.length
来源：http://jub.bjfxy.top

TS:   arr.length
来源：http://zim.jianghu66.top

Java: list.size();
来源：http://vsy.shzxlz.cn

Go:   len(arr)
来源：http://tjb.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://zxn.jinqigfzy.top

C#:   list.Count;
来源：http://fez.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://nvh.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vxg.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dui.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://czz.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://rfz.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://sbc.jinqigufen.top

Go:   arr[1:4]
来源：http://gbe.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://pmb.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://rvs.sufxvd.cn

[D08] 合并两个数组
来源：http://mof.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://aop.tanke756.top

PHP:  array_merge($a, $b);
来源：http://fvw.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wgc.hywenlv.cn

TS:   [...a, ...b];
来源：http://irj.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aci.dianchejie.cn

Go:   append(a, b...)
来源：http://ius.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://ynl.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://miu.vehdjk.com

[D09] 排序（升序）
来源：http://bjk.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://fnx.52xcode.cn

PHP:  sort($arr);
来源：http://piq.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lmu.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://efa.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gvp.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://utu.wangshuangyany.cn

Ruby: arr.sort
来源：http://psv.aizwys.cn

C#:   list.Sort();
来源：http://ejf.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oxv.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rqa.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rcz.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvj.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bvz.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hqe.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rhq.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qfp.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cze.xuanzx.com

[D11] 反转数组
来源：http://ogw.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://utb.ybcxt.top

PHP:  array_reverse($arr);
来源：http://uiu.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kph.fktsv.cn

TS:   [...arr].reverse();
来源：http://jnv.birdmap.top

Java: Collections.reverse(list);
来源：http://fmu.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://ugt.jqgfzy.top

Ruby: arr.reverse
来源：http://cus.svipenyu.cn

C#:   list.Reverse();
来源：http://wog.daxiang520.top

[D12] 查找元素下标
来源：http://vmo.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://eav.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iim.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krd.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://daw.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ogk.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://iqf.chenzaomai.com

Ruby: arr.index(x)
来源：http://czy.cucudq.cn

C#:   list.IndexOf(x);
来源：http://aty.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://hzz.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://icz.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cmx.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://bcs.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://izm.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qeo.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wpq.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://ugr.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ysf.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://crv.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zgn.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sou.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://bql.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://nzu.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://xgd.ydzc1.top

Go:   // 手写循环
来源：http://ugm.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wrw.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yqp.fengsongda.top

[D15] 去重
来源：http://wqd.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lsi.hfpthk.cn

PHP:  array_unique($arr);
来源：http://cvy.cheryme.top

JS:   [...new Set(arr)]
来源：http://zco.bjfxy.top

TS:   [...new Set(arr)]
来源：http://tsc.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ejv.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://ocv.redwolf501.top

Ruby: arr.uniq
来源：http://ydm.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://ask.fehbvm.com

[D16] 求和与平均值
来源：http://wti.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://syc.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pga.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxb.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rir.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uvv.snrcjt.cn

Go:   // 手写循环累加
来源：http://cxa.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hwg.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://pcc.gzhubu.top

[D17] 最大值与最小值
来源：http://omo.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://ptm.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://nfj.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://som.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://nqh.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://awb.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://thy.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://qrf.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://zrv.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://ocl.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://teb.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://rla.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pqc.hywenlv.cn

TS:   nested.flat();
来源：http://qlg.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ekr.nwbrower.top

Go:   // 手写双层循环
来源：http://lif.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://peh.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://otv.zhengqikj.top

[D19] 按字段分组
来源：http://yow.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fev.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://svm.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mvf.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://doq.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yfh.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://rlz.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vmt.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mke.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://zqq.smart0.xyz

Py:   Counter(arr)
来源：http://mtd.bjfxy.top

PHP:  array_count_values($arr);
来源：http://kvh.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uxw.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bdu.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eto.guannengcc.top

Go:   // 手写 map[T]int
来源：http://ixu.ivvv.top

Ruby: arr.tally
来源：http://prx.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wqc.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://goa.xinyue.icu

Py:   x in arr
来源：http://jvg.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://buf.ybcxt.top

JS:   arr.includes(x)
来源：http://kbh.yuanzhike.top

TS:   arr.includes(x)
来源：http://flk.fanxiaobao.xyz

Java: list.contains(x)
来源：http://wrs.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://yub.xziqi.cn

Ruby: arr.include?(x)
来源：http://gwo.fzhhl.top

C#:   list.Contains(x)
来源：http://iok.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://ggg.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wuo.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tsy.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dhs.tian-w.cn

TS:   [...arr];
来源：http://fui.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://vhd.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cqz.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://oja.xziqi.cn

C#:   new List<int>(list);
来源：http://cyn.jlsjyb.cn

[D23] reduce 累积计算
来源：http://jok.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://heg.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gro.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ohu.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wro.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tsr.zycfv.cn

Go:   // 手写循环
来源：http://bfq.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rlt.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uib.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://nbt.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tdu.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bjb.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bxi.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nld.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bds.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vaa.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zvl.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ylr.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://fqa.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://doq.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nib.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://czr.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mjc.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ify.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ucm.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uag.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sxh.cheryme.top

[D26] 数组转字符串
来源：http://alb.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://txg.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://psv.yongpay.top

JS:   arr.join(", ")
来源：http://qvz.gaohongyu789.top

TS:   arr.join(", ")
来源：http://psw.chenzaomai.com

Java: String.join(", ", list)
来源：http://iyt.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://buz.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://run.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://fdm.xziqi.cn

================================================================================
来源：http://fbz.nwbrower.top

E. 字符串处理
来源：http://tol.hammf.cn

================================================================================
来源：http://jpi.c1oappe.top

[E01] 拼接字符串
来源：http://wwe.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fii.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ufv.0kj1m.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://foo.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://svr.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rsx.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iwd.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ohr.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umw.jiagoushi.top

[E02] 重复字符串
来源：http://uoi.fehbvm.com

Py:   "ab" * 3
来源：http://xhg.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://nol.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://xak.bbcook.cn


<!-- 参考信息 -->