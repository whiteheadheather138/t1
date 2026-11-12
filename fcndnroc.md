代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://wnl.chenzaomai.com

C#:   using System.Text;
来源：http://olp.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://sxg.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://tco.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://dhe.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://udx.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://hji.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uxt.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://sbv.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://has.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://txw.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://sdk.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwz.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ala.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://szw.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgm.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://idv.cheryme.top

Go:   func add(a, b int) int
来源：http://wow.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://knp.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qzw.shangyingyoupin.top

[C14] 泛型函数
来源：http://sbl.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vll.hcnkem.com

PHP:  // 无泛型
来源：http://yny.andypj.xyz

JS:   // 无泛型
来源：http://ouy.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yhi.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vss.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://btt.ivvv.top

Ruby: # 无泛型
来源：http://naa.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mot.xuanzx.com

[C15] 解构 / 展开参数
来源：http://bqy.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hoz.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://uxz.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gyu.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kaf.jinghuilouyu.cn

Java: // 无解构
来源：http://rry.yuxming.cn

Go:   // 无解构
来源：http://xgo.316326.xyz

Ruby: a, b = pair
来源：http://jeu.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://ptt.epnwcf.com

[C16] 函数 / 方法重载
来源：http://dhk.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hix.jyoumei.cn

PHP:  // 无重载
来源：http://iwk.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qjp.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://tfg.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pzm.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://sjl.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://vgf.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qrc.mhx1999.top

================================================================================
来源：http://ebs.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://jsw.fktsv.cn

================================================================================
来源：http://eba.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://kvy.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://inf.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qan.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jrf.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lfh.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzt.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://otq.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://hps.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ryn.gzhubu.top

[D02] 追加元素到末尾
来源：http://uvk.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ldz.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xqi.hammf.cn

JS:   arr.push(4);
来源：http://pzv.xuanzx.com

TS:   arr.push(4);
来源：http://hva.vehdjk.com

Java: list.add(4);
来源：http://ulj.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://pdj.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://gbi.tianlin.xyz

C#:   list.Add(4);
来源：http://pes.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://ocq.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://xxa.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xne.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eaw.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://tvx.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://cxr.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bwd.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rsl.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://jqr.vehdjk.com

[D04] 删除元素
来源：http://oxu.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bly.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bfj.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wwh.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://hmc.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bbq.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hyu.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jgr.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mgw.daxiang520.top

[D05] 访问与修改元素
来源：http://wtl.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fut.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jss.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iud.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://fam.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://kpn.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://dki.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mqo.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pez.cqqwz.cn

[D06] 数组长度
来源：http://gbr.cashguo.top

Py:   len(arr)
来源：http://wlo.zdbjq.cn

PHP:  count($arr);
来源：http://gfn.yj20258.top

JS:   arr.length
来源：http://sbc.hnxiangtu.top

TS:   arr.length
来源：http://ldi.ivvv.top

Java: list.size();
来源：http://nth.aizwys.cn

Go:   len(arr)
来源：http://hxj.uphjek.com

Ruby: arr.length; arr.size
来源：http://tmx.hcnkem.com

C#:   list.Count;
来源：http://toj.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://srx.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cgv.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://oji.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://lhd.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://axo.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://yow.chenjidiqi.icu

Go:   arr[1:4]
来源：http://hms.dianchejie.cn

Ruby: arr[1, 3]
来源：http://ttc.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://cms.zhixingplan.top

[D08] 合并两个数组
来源：http://gpq.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://cgz.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://tmr.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bwz.ydzc1.top

TS:   [...a, ...b];
来源：http://bmg.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://slm.jianghu66.top

Go:   append(a, b...)
来源：http://nhy.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://qte.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://wtr.chenjidiqi.icu

[D09] 排序（升序）
来源：http://tyj.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://raw.ctjpmb.com

PHP:  sort($arr);
来源：http://kml.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://clm.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wct.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wru.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://msm.52xcode.cn

Ruby: arr.sort
来源：http://mwa.havefunace.top

C#:   list.Sort();
来源：http://mlt.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hax.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wiv.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcj.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kko.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nzm.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ceq.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cgm.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zjr.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ftp.xziqi.cn

[D11] 反转数组
来源：http://ozd.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxs.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://rcs.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yjo.ehwqpu.com

TS:   [...arr].reverse();
来源：http://bkl.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://kkd.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://wfw.birdmap.top

Ruby: arr.reverse
来源：http://tkc.xuanzx.com

C#:   list.Reverse();
来源：http://tlv.svipenyu.cn

[D12] 查找元素下标
来源：http://rez.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://xho.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tsd.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmx.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dhg.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xuu.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://gij.gaohongyu789.top

Ruby: arr.index(x)
来源：http://wul.daxiang520.top

C#:   list.IndexOf(x);
来源：http://nxe.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://jdc.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lso.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eat.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://opz.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://iyh.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://myo.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oqj.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://nau.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jdl.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://vll.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oxv.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ubr.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://xpp.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://eoz.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tyt.shanyushiyangtech.top

Go:   // 手写循环
来源：http://tuo.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://zop.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://air.hfpthk.cn

[D15] 去重
来源：http://mip.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lza.sysykeji.top

PHP:  array_unique($arr);
来源：http://kqn.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://yso.sysykeji.top

TS:   [...new Set(arr)]
来源：http://ybv.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://klg.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zgr.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://umw.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://wpj.zdqjudy.top

[D16] 求和与平均值
来源：http://kzy.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iih.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cfi.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://emr.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmb.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwu.hammf.cn

Go:   // 手写循环累加
来源：http://neo.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gqu.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://zsw.nwbrower.top

[D17] 最大值与最小值
来源：http://atw.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://wdp.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://tff.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eqz.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://baj.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhs.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bgq.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://eek.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://vtk.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://zhu.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ica.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://www.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cws.yuanzhike.top

TS:   nested.flat();
来源：http://wxk.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vga.cashguo.top

Go:   // 手写双层循环
来源：http://ofw.c1oappe.top

Ruby: nested.flatten
来源：http://pzb.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jzm.daxiang520.top

[D19] 按字段分组
来源：http://vsf.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xhp.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tzn.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kfv.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://cul.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xtz.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://xkz.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kcg.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izx.316326.xyz

[D20] 统计每个元素出现次数
来源：http://kpa.xuetiantiany.cn

Py:   Counter(arr)
来源：http://upv.yonumen.top

PHP:  array_count_values($arr);
来源：http://mtk.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwm.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eiw.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://byd.birdmap.top

Go:   // 手写 map[T]int
来源：http://ait.shuidangran.top

Ruby: arr.tally
来源：http://muc.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwc.fengsongda.top

[D21] 判断是否包含某元素
来源：http://fah.9152youxi.cn

Py:   x in arr
来源：http://pgg.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://sma.hnqzz.top

JS:   arr.includes(x)
来源：http://neu.zhoulong.xyz

TS:   arr.includes(x)
来源：http://gwf.cqqwz.cn

Java: list.contains(x)
来源：http://lui.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://mmy.yuxming.cn

Ruby: arr.include?(x)
来源：http://znt.gotoacloud.top

C#:   list.Contains(x)
来源：http://ggr.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://oim.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mrc.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://alg.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vao.xziqi.cn

TS:   [...arr];
来源：http://gsy.mhx1999.top

Java: new ArrayList<>(list);
来源：http://mqz.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://fxx.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://jbc.chenzaomai.com

C#:   new List<int>(list);
来源：http://dbo.snrcjt.cn

[D23] reduce 累积计算
来源：http://nej.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hmb.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bet.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://quk.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nka.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nvt.zhengqikj.top

Go:   // 手写循环
来源：http://ivw.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xar.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tla.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://iiw.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cmo.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wvw.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rmn.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bmb.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://myy.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gns.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwq.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ezo.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://ivm.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bds.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bgq.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wvd.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fea.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cmk.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lar.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxt.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqa.vehdjk.com

[D26] 数组转字符串
来源：http://ynv.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://utp.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://hkj.guannengcc.top

JS:   arr.join(", ")
来源：http://ztj.jinqigufen.top

TS:   arr.join(", ")
来源：http://dec.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://yye.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://qir.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://ceb.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://ats.tian-w.cn

================================================================================
来源：http://vfx.fehbvm.com

E. 字符串处理
来源：http://ldq.shuidangran.top

================================================================================
来源：http://zeu.yj20258.top

[E01] 拼接字符串
来源：http://lvr.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wya.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dbt.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oah.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://myd.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jvn.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://smb.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xds.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ocd.xuetiantiany.cn

[E02] 重复字符串
来源：http://ahg.cucudq.cn

Py:   "ab" * 3
来源：http://oos.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://rna.epnwcf.com

JS:   "ab".repeat(3)
来源：http://rqd.bbcook.cn


<!-- 参考信息 -->