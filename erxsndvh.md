代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpy.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fne.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wds.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgz.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://qbj.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://qlr.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ghb.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://izh.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://nui.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bgj.ydjk.org.cn

PHP:  // 无泛型
来源：http://kwu.hysaishi.cn

JS:   // 无泛型
来源：http://jpe.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hid.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lnp.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tri.uphjek.com

Ruby: # 无泛型
来源：http://woa.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uum.ydzc1.top

[C15] 解构 / 展开参数
来源：http://hwk.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hux.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://cqi.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nso.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yad.aizwys.cn

Java: // 无解构
来源：http://aig.redwolf501.top

Go:   // 无解构
来源：http://orp.cdnleiting.top

Ruby: a, b = pair
来源：http://hxj.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://lla.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://oxu.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://odl.zhengqikj.top

PHP:  // 无重载
来源：http://zyt.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://xls.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://aew.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vlr.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://zkt.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://tut.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://urj.epnwcf.com

================================================================================
来源：http://nuo.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://vaa.jiagoushi.top

================================================================================
来源：http://mix.fehbvm.com

[D01] 创建数组 / 列表
来源：http://hux.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lkv.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dev.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wko.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ymy.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bvw.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://mch.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://ckn.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oct.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://qrq.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ifi.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dlc.zhixingplan.top

JS:   arr.push(4);
来源：http://kwi.zhijiandao.cn

TS:   arr.push(4);
来源：http://qlc.hnxiangtu.top

Java: list.add(4);
来源：http://rkb.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://ecd.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://xnx.tanke756.top

C#:   list.Add(4);
来源：http://boz.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://dot.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://wko.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cgo.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jij.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://uzp.sjlbkw.cn

Java: list.add(0, 0);
来源：http://fod.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://mrb.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sjw.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://uyu.fanxiaobao.xyz

[D04] 删除元素
来源：http://fan.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yrx.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wcj.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://olh.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://boz.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lee.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://smo.cdnleiting.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://slq.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jqi.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://rro.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvu.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wnp.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rnc.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://neq.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://jsb.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://gys.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uyw.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wlj.vehdjk.com

[D06] 数组长度
来源：http://sqz.dashuyun.cn

Py:   len(arr)
来源：http://kbw.epnwcf.com

PHP:  count($arr);
来源：http://sib.cqqwz.cn

JS:   arr.length
来源：http://wgi.guannengcc.top

TS:   arr.length
来源：http://jkt.gzhubu.top

Java: list.size();
来源：http://lgm.xinyue.icu

Go:   len(arr)
来源：http://wsx.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://ryp.fehbvm.com

C#:   list.Count;
来源：http://uxy.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://ssr.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bnk.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nie.pycfn.com

JS:   arr.slice(1, 4);
来源：http://blw.yongpay.top

TS:   arr.slice(1, 4);
来源：http://iho.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://lvl.birdmap.top

Go:   arr[1:4]
来源：http://owo.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://wec.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://muu.jqgfzy.top

[D08] 合并两个数组
来源：http://lce.tian-w.cn

Py:   a + b;  a.extend(b)
来源：http://wgl.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://dpe.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ftw.jianghu66.top

TS:   [...a, ...b];
来源：http://xzu.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://egk.hnqzz.top

Go:   append(a, b...)
来源：http://rwy.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://dlp.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://kiz.yonumen.top

[D09] 排序（升序）
来源：http://nyb.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://wjz.zdqjudy.top

PHP:  sort($arr);
来源：http://eta.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yhf.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xyd.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cqz.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtv.haohaochexian.top

Ruby: arr.sort
来源：http://jix.pycfn.com

C#:   list.Sort();
来源：http://zfz.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fot.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ihy.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bdp.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltr.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rdo.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ddq.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bir.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mou.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nrl.jianghu66.top

[D11] 反转数组
来源：http://ysf.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://pdg.fktsv.cn

PHP:  array_reverse($arr);
来源：http://udq.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mgm.chenzaomai.com

TS:   [...arr].reverse();
来源：http://kwx.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://jct.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://yys.jyoumei.cn

Ruby: arr.reverse
来源：http://utg.nanxuanxn.top

C#:   list.Reverse();
来源：http://rha.zhijiandao.cn

[D12] 查找元素下标
来源：http://bgm.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://tol.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ylp.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eoa.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jlp.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://glc.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://luo.hammf.cn

Ruby: arr.index(x)
来源：http://zfp.hesvh.cn

C#:   list.IndexOf(x);
来源：http://shj.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://cuo.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yxw.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://emo.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://wol.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://emi.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lnv.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ngv.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://zkd.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cff.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://vtp.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pnn.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zqu.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://axs.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://yav.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xzv.ivvv.top

Go:   // 手写循环
来源：http://lwh.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://yud.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ysf.cashguo.top

[D15] 去重
来源：http://eoy.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lyb.xylfe.cn

PHP:  array_unique($arr);
来源：http://cst.meibo888.top

JS:   [...new Set(arr)]
来源：http://qxy.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://ycl.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://niq.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ipo.9152youxi.cn

Ruby: arr.uniq
来源：http://leg.havefunace.top

C#:   list.Distinct().ToList()
来源：http://atv.yangfankeji.com

[D16] 求和与平均值
来源：http://dsk.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gfg.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fnj.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cjd.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wif.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://csm.zhengqikj.top

Go:   // 手写循环累加
来源：http://wws.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://viz.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://qhr.c1oappe.top

[D17] 最大值与最小值
来源：http://owx.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://teh.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://dfg.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ykc.yuxming.cn

TS:   Math.max(...arr);
来源：http://woc.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rwc.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://efa.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://jxo.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://bel.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://rzg.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xbs.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://wdx.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ntq.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://tih.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vdj.xinyue.icu

Go:   // 手写双层循环
来源：http://nju.yangfankeji.com

Ruby: nested.flatten
来源：http://qju.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jsr.sxryk.cn

[D19] 按字段分组
来源：http://mct.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://doy.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uhh.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bam.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wbl.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jhh.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://pbi.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://cdv.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yge.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://ccr.hesvh.cn

Py:   Counter(arr)
来源：http://iat.daxiang520.top

PHP:  array_count_values($arr);
来源：http://muf.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvm.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yrz.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hgp.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://gud.zhoulong.xyz

Ruby: arr.tally
来源：http://ool.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hxr.cashguo.top

[D21] 判断是否包含某元素
来源：http://hxq.cashguo.top

Py:   x in arr
来源：http://tau.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://fol.wangdashe.top

JS:   arr.includes(x)
来源：http://mkm.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://bsc.shuidangran.top

Java: list.contains(x)
来源：http://wlv.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://nya.havefunace.top

Ruby: arr.include?(x)
来源：http://oya.hywenlv.cn

C#:   list.Contains(x)
来源：http://vsb.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://brk.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rez.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kcf.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ywt.hysaishi.cn

TS:   [...arr];
来源：http://zow.yfazqb.com

Java: new ArrayList<>(list);
来源：http://vit.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://zae.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://yni.cqqwz.cn

C#:   new List<int>(list);
来源：http://sbc.snrcjt.cn

[D23] reduce 累积计算
来源：http://zxi.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://azk.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://djx.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyv.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fmq.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tbd.yueranfly.top

Go:   // 手写循环
来源：http://amn.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://whs.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yfv.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://tft.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://opd.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nhc.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qzx.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jnx.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xqw.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cwl.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gfn.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rtj.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://rts.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jfg.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qok.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vqm.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lsv.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nox.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ezm.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oau.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://inx.uphjek.com

[D26] 数组转字符串
来源：http://tjm.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://sqt.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://ufk.ctjpmb.com

JS:   arr.join(", ")
来源：http://kyy.quarkkingdee.top

TS:   arr.join(", ")
来源：http://fta.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://fab.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://dgc.aizwys.cn

Ruby: arr.join(", ")
来源：http://fzc.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://jzt.yj202588.top

================================================================================
来源：http://yni.jqgfzy.top

E. 字符串处理
来源：http://zgg.xuanzx.com

================================================================================
来源：http://jhr.fzhhl.top

[E01] 拼接字符串
来源：http://ckd.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gbr.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hmh.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxq.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wcx.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rha.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mjl.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jjc.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ujt.cucudq.cn

[E02] 重复字符串
来源：http://nhr.gotoacloud.top

Py:   "ab" * 3
来源：http://dbw.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://wag.sxryk.cn

JS:   "ab".repeat(3)
来源：http://fps.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://piy.yuxming.cn

Java: "ab".repeat(3)
来源：http://pew.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://zvw.yueranfly.top

Ruby: "ab" * 3
来源：http://qlp.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uus.fktsv.cn

[E03] 截取子串
来源：http://swz.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://riw.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://buh.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lku.guannengcc.top

TS:   s.slice(1, 4)
来源：http://vtd.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://mdf.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mhq.shanyushiyangkeji.top


<!-- 参考信息 -->