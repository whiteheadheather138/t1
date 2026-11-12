代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ywd.316326.xyz

Go:   func add(a, b int) int
来源：http://uax.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwp.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hxf.hysaishi.cn

[C14] 泛型函数
来源：http://lck.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mpy.mhx1999.top

PHP:  // 无泛型
来源：http://wqt.meibo888.top

JS:   // 无泛型
来源：http://tao.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kvf.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rwg.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dop.pengpengdd.cyou

Ruby: # 无泛型
来源：http://pmo.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kbo.tanke756.top

[C15] 解构 / 展开参数
来源：http://rkt.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bxa.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://gxb.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lpc.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://quw.zhiwuduotai.top

Java: // 无解构
来源：http://trz.shanyushiyangkeji.top

Go:   // 无解构
来源：http://twz.snrcjt.cn

Ruby: a, b = pair
来源：http://mrg.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://jzr.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://odp.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zas.guowangkeji.top

PHP:  // 无重载
来源：http://byl.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wmy.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://lke.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pju.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://tzs.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://cys.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eqb.bbcook.cn

================================================================================
来源：http://yme.yongpay.top

D. 数组 / 列表 / 集合
来源：http://pzj.yvedp.cn

================================================================================
来源：http://mii.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://pgr.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xtl.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kio.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://djp.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://uwy.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://axq.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://aat.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://kzu.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://urs.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://xfj.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mgp.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dcn.hnqzz.top

JS:   arr.push(4);
来源：http://haz.daria6918.cn

TS:   arr.push(4);
来源：http://wqc.vqdsnc.cn

Java: list.add(4);
来源：http://aye.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://ixt.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://eoc.ydjk.org.cn

C#:   list.Add(4);
来源：http://lwj.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://bkz.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://rfn.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwn.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://izt.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://bio.andypj.xyz

Java: list.add(0, 0);
来源：http://pby.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://fih.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://scu.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://ylk.mhx1999.top

[D04] 删除元素
来源：http://jyz.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sdx.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://you.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wwy.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://wpl.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eff.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vsy.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wyt.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hiq.jlsjyb.cn

[D05] 访问与修改元素
来源：http://xmn.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ogm.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qun.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://znx.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://xkc.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://mrq.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://cjp.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://suf.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aen.wangshuangyany.cn

[D06] 数组长度
来源：http://opv.yj20258888.top

Py:   len(arr)
来源：http://sdq.shangyingyoupin.top

PHP:  count($arr);
来源：http://pxi.vqdsnc.cn

JS:   arr.length
来源：http://dtf.yvedp.cn

TS:   arr.length
来源：http://snu.smart0.xyz

Java: list.size();
来源：http://lkk.chenzaomai.com

Go:   len(arr)
来源：http://vaq.uphjek.com

Ruby: arr.length; arr.size
来源：http://lwa.yj20258888.top

C#:   list.Count;
来源：http://rnq.cashguo.top

[D07] 切片 / 取子数组
来源：http://alz.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jji.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hww.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://czy.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://lwr.sysykeji.top

Java: list.subList(1, 4);
来源：http://hck.dianchejie.cn

Go:   arr[1:4]
来源：http://mcf.zhixingplan.top

Ruby: arr[1, 3]
来源：http://gla.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://rsg.yongpay.top

[D08] 合并两个数组
来源：http://dau.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://ahh.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://quv.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://lou.snrcjt.cn

TS:   [...a, ...b];
来源：http://nmo.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://egf.svipenyu.cn

Go:   append(a, b...)
来源：http://teg.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://gzl.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://mov.nwbrower.top

[D09] 排序（升序）
来源：http://qvl.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://fez.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://bib.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tsp.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://awv.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ohc.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pqe.shzxlz.cn

Ruby: arr.sort
来源：http://whc.sxryk.cn

C#:   list.Sort();
来源：http://tsq.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fcv.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sxd.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqw.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gug.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cas.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://crz.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cry.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cyo.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mgy.yuanzhike.top

[D11] 反转数组
来源：http://vvy.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://uhh.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://eal.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cfz.shzxlz.cn

TS:   [...arr].reverse();
来源：http://wen.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://jwo.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://rgz.zdqjudy.top

Ruby: arr.reverse
来源：http://gvu.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://zcn.yfazqb.com

[D12] 查找元素下标
来源：http://nmu.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://zbj.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cig.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xib.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zzu.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://drx.cashguo.top

Go:   slices.Index(arr, x)
来源：http://yik.aibaodan.cn

Ruby: arr.index(x)
来源：http://enn.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://xum.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://qec.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uiw.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xcg.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://epv.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://qnb.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mae.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmm.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://faz.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kcz.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://nkv.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mzf.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rgg.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://hdk.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://qhe.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fim.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://tun.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ynm.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rfq.chenjidiqi.icu

[D15] 去重
来源：http://pgf.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://znv.cdnleiting.top

PHP:  array_unique($arr);
来源：http://idp.smart0.xyz

JS:   [...new Set(arr)]
来源：http://zgs.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://yjq.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hkw.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://mrs.hnqzz.top

Ruby: arr.uniq
来源：http://hup.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://cov.gaohongyu789.top

[D16] 求和与平均值
来源：http://qav.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cif.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhp.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://emk.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rim.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://woa.yonumen.top

Go:   // 手写循环累加
来源：http://omo.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exe.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://hhv.xylfe.cn

[D17] 最大值与最小值
来源：http://rdu.birdmap.top

Py:   max(arr);  min(arr)
来源：http://uwi.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://btk.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://geo.ppjwa.cn

TS:   Math.max(...arr);
来源：http://qff.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://wqn.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fci.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://fkq.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://hos.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://wvz.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xpo.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://llo.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qjj.tarul.cn

TS:   nested.flat();
来源：http://fkf.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xor.zhixingplan.top

Go:   // 手写双层循环
来源：http://dvf.hywenlv.cn

Ruby: nested.flatten
来源：http://olt.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zfz.haohaochexian.top

[D19] 按字段分组
来源：http://jbj.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ejy.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxd.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gre.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uaj.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://otp.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://ueh.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zqr.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfz.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://ivf.nwbrower.top

Py:   Counter(arr)
来源：http://suc.yj20258888.top

PHP:  array_count_values($arr);
来源：http://wbo.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjm.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://egf.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xhh.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://ubv.316326.xyz

Ruby: arr.tally
来源：http://tmo.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmx.cucudq.cn

[D21] 判断是否包含某元素
来源：http://szb.yvedp.cn

Py:   x in arr
来源：http://aut.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://aii.sufxvd.cn

JS:   arr.includes(x)
来源：http://zfo.hnxiangtu.top

TS:   arr.includes(x)
来源：http://jwr.yangfankeji.com

Java: list.contains(x)
来源：http://rfj.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://ziz.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://zll.jlsjyb.cn

C#:   list.Contains(x)
来源：http://rhb.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://qav.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://slr.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qnm.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pki.jinyuanbaomall.cn

TS:   [...arr];
来源：http://pbl.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://flz.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vhd.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://zrg.snrcjt.cn

C#:   new List<int>(list);
来源：http://odn.yvedp.cn

[D23] reduce 累积计算
来源：http://upy.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mva.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kyl.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qsp.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mhb.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gfd.ctjpmb.com

Go:   // 手写循环
来源：http://crp.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cfa.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vqe.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://vjw.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vxt.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bvk.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mhc.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hhe.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yay.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jkt.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zpx.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tza.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://ozl.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rwr.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kew.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://njn.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bzx.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yiv.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ncj.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ywh.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cug.feifeiyinyue.top

[D26] 数组转字符串
来源：http://uvt.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://mcq.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://ruc.fktsv.cn

JS:   arr.join(", ")
来源：http://qvt.dianchejie.cn

TS:   arr.join(", ")
来源：http://gsd.yangfankeji.com

Java: String.join(", ", list)
来源：http://krc.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://rdy.yuanzhike.top

Ruby: arr.join(", ")
来源：http://ytx.aizwys.cn

C#:   string.Join(", ", list)
来源：http://qug.svipenyu.cn

================================================================================
来源：http://hns.daria6918.cn

E. 字符串处理
来源：http://gvz.hongshengwenyu.top

================================================================================
来源：http://vvo.ybcxt.top

[E01] 拼接字符串
来源：http://nnw.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jlz.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pci.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://azg.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qta.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oza.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ien.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ufc.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tga.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://bpo.fzhhl.top

Py:   "ab" * 3
来源：http://zum.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://vtc.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://tor.yj20258.top

TS:   "ab".repeat(3)
来源：http://hzr.tarul.cn

Java: "ab".repeat(3)
来源：http://ooq.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://dmi.pycfn.com

Ruby: "ab" * 3
来源：http://vdf.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ico.hnxiangtu.top

[E03] 截取子串
来源：http://yxu.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fhy.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zeg.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zmz.xinyue.icu

TS:   s.slice(1, 4)
来源：http://cbq.chenzaomai.com

Java: s.substring(1, 4)
来源：http://doc.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vhf.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://coh.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://ndp.c1oappe.top

[E04] 查找子串位置
来源：http://obl.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://seu.zhoulong.xyz


<!-- 参考信息 -->