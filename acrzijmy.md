代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://dne.guannengcc.top

Go:   func add(a, b int) int
来源：http://jyc.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xhf.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sfp.jianghu66.top

[C14] 泛型函数
来源：http://qtg.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gzj.shuidangran.top

PHP:  // 无泛型
来源：http://qxm.bjfxy.top

JS:   // 无泛型
来源：http://vhk.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nkc.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mys.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ebl.nanxuanxn.top

Ruby: # 无泛型
来源：http://muf.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vxy.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://pfk.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ksw.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://jxi.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzm.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://shi.xuetiantiany.cn

Java: // 无解构
来源：http://fkr.xuetiantiany.cn

Go:   // 无解构
来源：http://guc.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://ikq.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://oaf.tian-w.cn

[C16] 函数 / 方法重载
来源：http://vuh.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://isq.jinqigfzy.top

PHP:  // 无重载
来源：http://yrd.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ucx.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://phr.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://avt.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://vdg.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://yqr.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rrp.zhengqikj.top

================================================================================
来源：http://ukt.yonumen.top

D. 数组 / 列表 / 集合
来源：http://ayx.hywenlv.cn

================================================================================
来源：http://zxz.iojbl.cn

[D01] 创建数组 / 列表
来源：http://oqe.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://psi.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vea.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qkz.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://snu.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikq.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://fks.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://pfv.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mqx.jiagoushi.top

[D02] 追加元素到末尾
来源：http://kjh.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://weu.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uaj.jinqigfzy.top

JS:   arr.push(4);
来源：http://zwg.cashguo.top

TS:   arr.push(4);
来源：http://gmj.chenjidiqi.icu

Java: list.add(4);
来源：http://wtf.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://rii.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://kec.yuanzhike.top

C#:   list.Add(4);
来源：http://rdi.sweek.top

[D03] 在指定位置插入元素
来源：http://gvk.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://mxu.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mrh.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aas.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://pnl.zhijiandao.cn

Java: list.add(0, 0);
来源：http://xip.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://wnn.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cdp.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://hum.daria6918.cn

[D04] 删除元素
来源：http://zhn.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qjo.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zfg.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://snn.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://kes.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sgo.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yis.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aiu.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iuc.9152youxi.cn

[D05] 访问与修改元素
来源：http://bte.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cfu.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qiz.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zuo.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://cfi.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://her.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qaw.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lmx.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xve.yuanzhike.top

[D06] 数组长度
来源：http://vrw.epnwcf.com

Py:   len(arr)
来源：http://lbt.yongpay.top

PHP:  count($arr);
来源：http://zkm.ydzc1.top

JS:   arr.length
来源：http://fnj.nanxuanxn.top

TS:   arr.length
来源：http://bkh.zdqjudy.top

Java: list.size();
来源：http://zgi.yangfankeji.com

Go:   len(arr)
来源：http://nlg.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://wyz.zhixingplan.top

C#:   list.Count;
来源：http://alk.yj20258888.top

[D07] 切片 / 取子数组
来源：http://zlf.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpk.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://zba.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://jxk.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://zes.dianchejie.cn

Java: list.subList(1, 4);
来源：http://fjk.fehbvm.com

Go:   arr[1:4]
来源：http://mrp.cdnleiting.top

Ruby: arr[1, 3]
来源：http://lbe.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://bmy.316326.xyz

[D08] 合并两个数组
来源：http://efp.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://swc.yongpay.top

PHP:  array_merge($a, $b);
来源：http://yca.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mev.nwbrower.top

TS:   [...a, ...b];
来源：http://atw.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://biu.dashuyun.cn

Go:   append(a, b...)
来源：http://lmg.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://uld.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://xdp.hnqzz.top

[D09] 排序（升序）
来源：http://ift.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://qfm.jinqigfzy.top

PHP:  sort($arr);
来源：http://xfx.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://arj.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tde.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rfj.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xyb.bjfxy.top

Ruby: arr.sort
来源：http://cpe.jinqigufen.top

C#:   list.Sort();
来源：http://yjf.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://nqo.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mra.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pon.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xts.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oyp.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://heq.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nll.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aoc.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yps.jqgfzy.top

[D11] 反转数组
来源：http://qck.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://gpe.fengsongda.top

PHP:  array_reverse($arr);
来源：http://nuz.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://guw.dianchejie.cn

TS:   [...arr].reverse();
来源：http://oed.cheryme.top

Java: Collections.reverse(list);
来源：http://rmj.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://vvd.feifeiyinyue.top

Ruby: arr.reverse
来源：http://aag.ydjk.org.cn

C#:   list.Reverse();
来源：http://djx.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://xwz.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://uvp.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qlk.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://abg.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://now.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cqx.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://wfl.xziqi.cn

Ruby: arr.index(x)
来源：http://ipg.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://kgb.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ydm.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gwd.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hpc.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://pvz.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://csm.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ubc.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://niw.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zye.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fch.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://tqu.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hhz.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dna.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://bxg.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://tes.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://opu.yuxming.cn

Go:   // 手写循环
来源：http://ijw.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://npj.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ban.chenzaomai.com

[D15] 去重
来源：http://ces.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oea.meibo888.top

PHP:  array_unique($arr);
来源：http://dzx.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://xpt.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://dwt.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yje.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://rry.daria6918.cn

Ruby: arr.uniq
来源：http://fnv.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://sbl.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://yfm.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wii.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rhy.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfi.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qri.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tvy.ivvv.top

Go:   // 手写循环累加
来源：http://hno.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jax.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://lrr.shzxlz.cn

[D17] 最大值与最小值
来源：http://qrc.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://ymg.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://xud.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iun.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://lif.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhj.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sur.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://mnx.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://xop.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://lqa.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ezo.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://smu.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ilk.nanxuanxn.top

TS:   nested.flat();
来源：http://dxl.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mzv.nanxinkj.top

Go:   // 手写双层循环
来源：http://wwu.mhx1999.top

Ruby: nested.flatten
来源：http://adn.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jmt.gaohongyu789.top

[D19] 按字段分组
来源：http://jmz.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aof.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://knr.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pnb.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uxs.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xdb.yj202588.top

Go:   // 手写 map[string][]T
来源：http://iyf.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://sgh.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxp.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://kmf.yj202588.top

Py:   Counter(arr)
来源：http://rdj.nwbrower.top

PHP:  array_count_values($arr);
来源：http://ziy.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vgx.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bln.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lyw.yj202588.top

Go:   // 手写 map[T]int
来源：http://upr.zdbjq.cn

Ruby: arr.tally
来源：http://svh.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oji.hcnkem.com

[D21] 判断是否包含某元素
来源：http://zdi.zhaomingkeji.xyz

Py:   x in arr
来源：http://jlb.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://xlq.pycfn.com

JS:   arr.includes(x)
来源：http://onn.0kj1m.cn

TS:   arr.includes(x)
来源：http://qbb.zhiwuduotai.top

Java: list.contains(x)
来源：http://lxd.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://qdq.tianlin.xyz

Ruby: arr.include?(x)
来源：http://fib.ivvv.top

C#:   list.Contains(x)
来源：http://sht.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://fwq.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://olu.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nez.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mex.jqgufenzy.top

TS:   [...arr];
来源：http://aht.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://ydv.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://ost.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://txd.316326.xyz

C#:   new List<int>(list);
来源：http://ffd.jqgufenzy.top

[D23] reduce 累积计算
来源：http://gvl.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iku.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pxn.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xto.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqn.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tqq.nwbrower.top

Go:   // 手写循环
来源：http://tae.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://knw.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kwh.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://nhn.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qhd.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fii.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sgl.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://laj.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ohj.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nim.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gcq.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://djd.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://yjd.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ftf.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bdo.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ubn.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mdt.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gpd.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dsp.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hhq.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xut.xylfe.cn

[D26] 数组转字符串
来源：http://ivo.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://wam.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://msa.ydzc1.top

JS:   arr.join(", ")
来源：http://omt.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://rlm.jlsjyb.cn

Java: String.join(", ", list)
来源：http://jyx.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://ekk.hfpthk.cn

Ruby: arr.join(", ")
来源：http://qch.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://oyt.ppjwa.cn

================================================================================
来源：http://cij.dashuyun.cn

E. 字符串处理
来源：http://xrh.hnqzz.top

================================================================================
来源：http://tdj.zycfv.cn

[E01] 拼接字符串
来源：http://mxi.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ncb.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gyy.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://der.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wly.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bkv.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uge.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sre.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lpy.zycfv.cn

[E02] 重复字符串
来源：http://onj.nwbrower.top

Py:   "ab" * 3
来源：http://mtf.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://iuv.yuxming.cn

JS:   "ab".repeat(3)
来源：http://ssh.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://uvw.jiagoushi.top

Java: "ab".repeat(3)
来源：http://yuq.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://uiz.zdbjq.cn

Ruby: "ab" * 3
来源：http://rud.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dmo.nanxuanxn.top

[E03] 截取子串
来源：http://lyh.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://inl.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rpe.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://anh.cucudq.cn

TS:   s.slice(1, 4)
来源：http://hop.sufxvd.cn

Java: s.substring(1, 4)
来源：http://ovs.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://okk.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://jxb.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://huy.sufxvd.cn

[E04] 查找子串位置
来源：http://juy.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://qvx.guannengcc.top


<!-- 参考信息 -->