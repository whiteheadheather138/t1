代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://asx.hongshengwenyu.top

C#:   using System.Text;
来源：http://pol.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://kao.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://zwy.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://dtq.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://tpr.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://ayi.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mes.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://nfx.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://buv.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nii.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://vul.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mab.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xho.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jnp.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zqy.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://mhi.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://nsq.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tom.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://wij.9152youxi.cn

[C14] 泛型函数
来源：http://cvx.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lcy.zdbjq.cn

PHP:  // 无泛型
来源：http://mec.yongpay.top

JS:   // 无泛型
来源：http://jhh.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://skb.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yvv.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kby.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://rnk.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://svu.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://ooq.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zju.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://kpv.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ffa.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hps.sjlbkw.cn

Java: // 无解构
来源：http://ydo.sufxvd.cn

Go:   // 无解构
来源：http://qmp.zhoulong.xyz

Ruby: a, b = pair
来源：http://mdt.nwbrower.top

C#:   var (a, b) = pair;
来源：http://urv.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://snf.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hht.birdmap.top

PHP:  // 无重载
来源：http://pbp.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gpr.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://psf.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://jbs.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://rzm.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://ifv.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://plw.redwolf501.top

================================================================================
来源：http://izc.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://nfw.zhijiandao.cn

================================================================================
来源：http://ejp.yj20258.top

[D01] 创建数组 / 列表
来源：http://xas.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dhr.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gho.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bli.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zpx.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jzq.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://ooe.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://lso.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ble.yangfankeji.com

[D02] 追加元素到末尾
来源：http://nmo.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qjn.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://akd.fzhhl.top

JS:   arr.push(4);
来源：http://kpn.hcnkem.com

TS:   arr.push(4);
来源：http://wsy.ppjwa.cn

Java: list.add(4);
来源：http://acy.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://kfo.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://rkn.tanke756.top

C#:   list.Add(4);
来源：http://oad.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://auf.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://hgh.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rjv.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ocj.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://ykg.daria6918.cn

Java: list.add(0, 0);
来源：http://qpv.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vnj.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oav.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://wdz.shzxlz.cn

[D04] 删除元素
来源：http://cuy.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lcv.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pxw.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uys.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://twy.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://alv.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwj.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rfj.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vak.tian-w.cn

[D05] 访问与修改元素
来源：http://zba.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hut.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qwo.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jou.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://vcd.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://nxz.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://etj.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qvu.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kug.redwolf501.top

[D06] 数组长度
来源：http://xxz.tian-w.cn

Py:   len(arr)
来源：http://pjc.uphjek.com

PHP:  count($arr);
来源：http://ybt.nanxinkj.top

JS:   arr.length
来源：http://zrr.gogol.net.cn

TS:   arr.length
来源：http://mnm.fzhhl.top

Java: list.size();
来源：http://ljh.ppjwa.cn

Go:   len(arr)
来源：http://hlw.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://eah.mhx1999.top

C#:   list.Count;
来源：http://txe.daxiang520.top

[D07] 切片 / 取子数组
来源：http://lzr.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mal.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://rtq.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://dcn.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://gmn.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://pid.yangfankeji.com

Go:   arr[1:4]
来源：http://wiy.guowangkeji.top

Ruby: arr[1, 3]
来源：http://vmn.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://fot.andypj.xyz

[D08] 合并两个数组
来源：http://ngl.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://jyp.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://oof.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://huw.c1oappe.top

TS:   [...a, ...b];
来源：http://qwv.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wja.zdqjudy.top

Go:   append(a, b...)
来源：http://pfu.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://jbz.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://wdv.ybcxt.top

[D09] 排序（升序）
来源：http://jrn.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ddr.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://knv.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xmc.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cel.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uvq.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uvz.haohaochexian.top

Ruby: arr.sort
来源：http://rvn.c1oappe.top

C#:   list.Sort();
来源：http://dfj.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uva.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tla.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bzm.jinqigfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cdh.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vjd.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rqs.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://myl.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ipm.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uow.ybcxt.top

[D11] 反转数组
来源：http://gwg.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://kcw.sxryk.cn

PHP:  array_reverse($arr);
来源：http://hez.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ole.chenzaomai.com

TS:   [...arr].reverse();
来源：http://umn.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://ujt.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://tso.havefunace.top

Ruby: arr.reverse
来源：http://hav.fzhhl.top

C#:   list.Reverse();
来源：http://dpe.epnwcf.com

[D12] 查找元素下标
来源：http://rxi.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://pqa.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xgg.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dnn.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwt.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ohv.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://ocd.cdnleiting.top

Ruby: arr.index(x)
来源：http://czf.bjfxy.top

C#:   list.IndexOf(x);
来源：http://drz.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://qkz.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpy.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzg.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://zno.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://cal.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jek.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ruk.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fjg.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ccx.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://dgu.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lzk.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://luk.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://isi.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://tnj.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ppn.tianlin.xyz

Go:   // 手写循环
来源：http://avx.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://myr.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ezp.nanxuanxn.top

[D15] 去重
来源：http://qhl.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://abj.yvedp.cn

PHP:  array_unique($arr);
来源：http://ckz.shuidangran.top

JS:   [...new Set(arr)]
来源：http://xgi.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://amb.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://upn.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://oxz.gaohongyu789.top

Ruby: arr.uniq
来源：http://qhi.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://gog.haohaochexian.top

[D16] 求和与平均值
来源：http://smh.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mak.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xjl.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixo.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://opd.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fpd.kuanghao11.cn

Go:   // 手写循环累加
来源：http://ebv.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ota.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://rbo.sxryk.cn

[D17] 最大值与最小值
来源：http://qiy.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://yng.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://jch.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pdn.cheryme.top

TS:   Math.max(...arr);
来源：http://pes.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qzm.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqk.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://ehr.yongpay.top

C#:   list.Max();  list.Min()
来源：http://eiv.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://buj.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://btm.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://scr.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pxa.ehwqpu.com

TS:   nested.flat();
来源：http://erg.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://snu.quarkkingdee.top

Go:   // 手写双层循环
来源：http://wyx.zhijiandao.cn

Ruby: nested.flatten
来源：http://nbm.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xen.tian-w.cn

[D19] 按字段分组
来源：http://ajq.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://agn.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yms.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vax.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://unv.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pja.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://vqj.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lcy.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cbx.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://ryu.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://nll.tanke756.top

PHP:  array_count_values($arr);
来源：http://gwf.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulc.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://stm.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tlj.hcnkem.com

Go:   // 手写 map[T]int
来源：http://kvj.gzhubu.top

Ruby: arr.tally
来源：http://hak.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nwc.wangdashe.top

[D21] 判断是否包含某元素
来源：http://qtf.jinqigfzy.top

Py:   x in arr
来源：http://kxt.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://lie.tian-w.cn

JS:   arr.includes(x)
来源：http://mnf.sjlbkw.cn

TS:   arr.includes(x)
来源：http://srh.hysaishi.cn

Java: list.contains(x)
来源：http://vox.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://nfm.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://oug.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://ivm.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://jlr.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jyv.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qcb.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvd.jqgufenzy.top

TS:   [...arr];
来源：http://gpq.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://exp.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://sdz.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://vka.fktsv.cn

C#:   new List<int>(list);
来源：http://zhn.sjlbkw.cn

[D23] reduce 累积计算
来源：http://skw.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://our.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wea.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zbf.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsu.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofx.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://koo.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://juv.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rig.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://mnh.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hiz.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yle.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iig.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lau.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zwl.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yaj.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ogr.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ywr.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://wic.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opg.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hwi.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yih.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nvu.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kkc.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://prz.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xhz.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://frj.birdmap.top

[D26] 数组转字符串
来源：http://xzm.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://edb.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://tug.redwolf501.top

JS:   arr.join(", ")
来源：http://dch.xuanzx.com

TS:   arr.join(", ")
来源：http://xvz.epnwcf.com

Java: String.join(", ", list)
来源：http://svh.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://egd.yj202588.top

Ruby: arr.join(", ")
来源：http://ieu.meibo888.top

C#:   string.Join(", ", list)
来源：http://jau.xuanzx.com

================================================================================
来源：http://wop.yfazqb.com

E. 字符串处理
来源：http://uqt.hnxiangtu.top

================================================================================
来源：http://gax.xuetiantiany.cn

[E01] 拼接字符串
来源：http://ybp.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wud.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aqo.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://szf.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://leq.guannengcc.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nnt.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://saf.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://quf.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gmk.fehbvm.com

[E02] 重复字符串
来源：http://ylv.hysaishi.cn

Py:   "ab" * 3
来源：http://hez.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://xav.nwbrower.top

JS:   "ab".repeat(3)
来源：http://ypc.smart0.xyz


<!-- 参考信息 -->