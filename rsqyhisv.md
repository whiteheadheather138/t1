代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://oma.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://ysl.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://ogz.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kqq.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://hcc.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://jbr.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://igd.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://jrc.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqx.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kue.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ryk.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://plu.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://bhi.0kj1m.cn

Go:   func add(a, b int) int
来源：http://exj.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qew.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://pfd.gaohongyu789.top

[C14] 泛型函数
来源：http://fah.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ntd.tian-w.cn

PHP:  // 无泛型
来源：http://rjf.zhixingplan.top

JS:   // 无泛型
来源：http://grg.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://twx.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hzw.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lta.316326.xyz

Ruby: # 无泛型
来源：http://uzr.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wah.jianghu66.top

[C15] 解构 / 展开参数
来源：http://nxk.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vjd.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://wsf.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wax.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vxh.xuetiantiany.cn

Java: // 无解构
来源：http://bxm.xylfe.cn

Go:   // 无解构
来源：http://mhl.aizwys.cn

Ruby: a, b = pair
来源：http://adm.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://chy.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://dnr.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qir.pengpengdd.cyou

PHP:  // 无重载
来源：http://byt.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wqx.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://qnn.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cac.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://ifb.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://mrc.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ias.xinyue.icu

================================================================================
来源：http://hya.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://hzm.pengpengdd.cyou

================================================================================
来源：http://teq.wangdashe.top

[D01] 创建数组 / 列表
来源：http://ayf.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xgd.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lsk.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kux.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uqp.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nov.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://hkh.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://ako.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vre.0kj1m.cn

[D02] 追加元素到末尾
来源：http://zny.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yst.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://neu.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://wrx.shzxlz.cn

TS:   arr.push(4);
来源：http://qgd.daria6918.cn

Java: list.add(4);
来源：http://vkb.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://boq.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://yzo.fehbvm.com

C#:   list.Add(4);
来源：http://evs.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://iwq.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://eia.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qkz.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://usl.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://ptn.aizwys.cn

Java: list.add(0, 0);
来源：http://sys.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sxv.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://agt.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://amh.yuxming.cn

[D04] 删除元素
来源：http://xqh.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://thk.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yuc.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vhj.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://gzx.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://evs.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zps.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xio.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wdd.fzhhl.top

[D05] 访问与修改元素
来源：http://ejn.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://epo.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qng.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nol.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://vsy.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://kns.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://mci.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tir.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sho.xinyue.icu

[D06] 数组长度
来源：http://bwt.jyoumei.cn

Py:   len(arr)
来源：http://ofd.gzhubu.top

PHP:  count($arr);
来源：http://apx.andypj.xyz

JS:   arr.length
来源：http://rrt.meibo888.top

TS:   arr.length
来源：http://vdv.52xcode.cn

Java: list.size();
来源：http://qht.ehwqpu.com

Go:   len(arr)
来源：http://saq.wangdashe.top

Ruby: arr.length; arr.size
来源：http://xmr.dianchejie.cn

C#:   list.Count;
来源：http://hjy.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://tsi.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jni.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://src.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://zpj.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://bsc.vehdjk.com

Java: list.subList(1, 4);
来源：http://ccl.xinyue.icu

Go:   arr[1:4]
来源：http://zvs.zycfv.cn

Ruby: arr[1, 3]
来源：http://pgz.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://mxi.sxryk.cn

[D08] 合并两个数组
来源：http://een.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://ysj.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://nic.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pla.ctjpmb.com

TS:   [...a, ...b];
来源：http://avc.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zmz.bbcook.cn

Go:   append(a, b...)
来源：http://wip.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://nri.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://dtc.chenzaomai.com

[D09] 排序（升序）
来源：http://uls.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ydq.guowangkeji.top

PHP:  sort($arr);
来源：http://bam.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jnl.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pra.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zrt.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgx.aizwys.cn

Ruby: arr.sort
来源：http://wjp.fengsongda.top

C#:   list.Sort();
来源：http://msh.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://hzb.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mhm.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pjd.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxz.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekr.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aqs.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tlj.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zkt.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vhu.fanxiaobao.xyz

[D11] 反转数组
来源：http://xrd.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://kvf.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://fjd.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eqc.haohaochexian.top

TS:   [...arr].reverse();
来源：http://zwf.jyoumei.cn

Java: Collections.reverse(list);
来源：http://uhy.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://nsv.xinyue.icu

Ruby: arr.reverse
来源：http://tpd.jinqigfzy.top

C#:   list.Reverse();
来源：http://xjv.jqgfzy.top

[D12] 查找元素下标
来源：http://lbq.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://txh.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://acw.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfe.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hva.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lzo.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://zum.cucudq.cn

Ruby: arr.index(x)
来源：http://tdf.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://ere.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://bum.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kzh.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzh.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://bzp.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://enc.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cxo.shangyingyoupin.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prw.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://zmm.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lat.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://hfs.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zsj.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cim.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://nwn.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://zsm.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://toe.wangshuangyany.cn

Go:   // 手写循环
来源：http://ptw.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://tps.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cnr.zdbjq.cn

[D15] 去重
来源：http://xoq.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qkt.c1oappe.top

PHP:  array_unique($arr);
来源：http://fgs.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://eaj.nwbrower.top

TS:   [...new Set(arr)]
来源：http://aeg.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gnm.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://ssw.ybcxt.top

Ruby: arr.uniq
来源：http://mur.sweek.top

C#:   list.Distinct().ToList()
来源：http://ucv.tian-w.cn

[D16] 求和与平均值
来源：http://vmz.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mvm.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwq.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jaw.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpr.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xbu.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://epg.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kys.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://ifz.sweek.top

[D17] 最大值与最小值
来源：http://hds.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://uls.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://dww.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kkk.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://jbd.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ggz.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ida.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://nxy.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://vnl.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://xtu.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ass.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://cwj.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://guf.smart0.xyz

TS:   nested.flat();
来源：http://mgr.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ivr.ivvv.top

Go:   // 手写双层循环
来源：http://jpq.hnqzz.top

Ruby: nested.flatten
来源：http://axd.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nmp.mhx1999.top

[D19] 按字段分组
来源：http://zre.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jzp.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://omd.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ntx.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xmu.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jrq.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://jif.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fpi.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pql.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://jlg.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://npq.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://jql.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abs.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrv.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jny.andypj.xyz

Go:   // 手写 map[T]int
来源：http://igt.ehwqpu.com

Ruby: arr.tally
来源：http://qar.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dlr.hammf.cn

[D21] 判断是否包含某元素
来源：http://sdb.yj20258888.top

Py:   x in arr
来源：http://rcq.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://iir.hysaishi.cn

JS:   arr.includes(x)
来源：http://kbe.vehdjk.com

TS:   arr.includes(x)
来源：http://uvd.jinqigufen.top

Java: list.contains(x)
来源：http://sny.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://kiz.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://yer.bjfxy.top

C#:   list.Contains(x)
来源：http://uix.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://xjh.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://din.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hhh.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwi.iojbl.cn

TS:   [...arr];
来源：http://rpd.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://atv.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://qkq.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://jwt.cashguo.top

C#:   new List<int>(list);
来源：http://zru.sxryk.cn

[D23] reduce 累积计算
来源：http://rgz.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://now.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://frm.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpi.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpl.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ttb.hongshengwenyu.top

Go:   // 手写循环
来源：http://roo.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fbo.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jqs.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://oks.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cps.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jvb.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://amm.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bbp.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tao.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ybe.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tfd.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ckc.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://qgh.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cge.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uli.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfr.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wal.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://okp.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tqq.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://paf.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gyv.fktsv.cn

[D26] 数组转字符串
来源：http://rzw.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://xcq.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://qmk.uphjek.com

JS:   arr.join(", ")
来源：http://kkj.cqqwz.cn

TS:   arr.join(", ")
来源：http://ehi.zhongyouzk.top

Java: String.join(", ", list)
来源：http://kti.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://kuv.gogol.net.cn

Ruby: arr.join(", ")
来源：http://yaw.cheryme.top

C#:   string.Join(", ", list)
来源：http://lvz.zhijiandao.cn

================================================================================
来源：http://pzi.tanke756.top

E. 字符串处理
来源：http://bcm.jlsjyb.cn

================================================================================
来源：http://uge.c1oappe.top

[E01] 拼接字符串
来源：http://guc.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gpp.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hfv.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vcp.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ykr.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bjb.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fqd.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hbs.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fis.yuanzhike.top

[E02] 重复字符串
来源：http://mlo.yanxiufei.cn

Py:   "ab" * 3
来源：http://znq.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://vxw.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://usq.hcnkem.com

TS:   "ab".repeat(3)
来源：http://ccy.bjfxy.top

Java: "ab".repeat(3)
来源：http://avl.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://gbr.xinyue.icu

Ruby: "ab" * 3
来源：http://wjk.fzhhl.top


<!-- 参考信息 -->