代发 wailian999

[C14] 泛型函数
来源：http://uww.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ryp.zhongyouzk.top

PHP:  // 无泛型
来源：http://hrk.yangfankeji.com

JS:   // 无泛型
来源：http://dob.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fkq.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rsn.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ktk.shuidangran.top

Ruby: # 无泛型
来源：http://owd.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xwy.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://pgo.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fia.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://pxp.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kkz.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nps.uphjek.com

Java: // 无解构
来源：http://fis.sjlbkw.cn

Go:   // 无解构
来源：http://mvh.feifeiyinyue.top

Ruby: a, b = pair
来源：http://qjc.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://gup.bbcook.cn

[C16] 函数 / 方法重载
来源：http://upz.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rbw.ybcxt.top

PHP:  // 无重载
来源：http://voh.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zkh.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://dxu.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://qxl.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://hrl.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://cdu.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oqz.tianlin.xyz

================================================================================
来源：http://fxp.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://dbe.redwolf501.top

================================================================================
来源：http://tdw.gzhubu.top

[D01] 创建数组 / 列表
来源：http://nqm.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fcj.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://isp.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dzz.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ccw.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xtd.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://jio.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://hwh.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mnw.cheryme.top

[D02] 追加元素到末尾
来源：http://qnb.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vlh.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pja.vehdjk.com

JS:   arr.push(4);
来源：http://bzg.hongshengwenyu.top

TS:   arr.push(4);
来源：http://www.zdqjudy.top

Java: list.add(4);
来源：http://vmr.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://ewu.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://uip.sysykeji.top

C#:   list.Add(4);
来源：http://soc.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://dph.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ftu.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rmf.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lys.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://eop.nwbrower.top

Java: list.add(0, 0);
来源：http://bwy.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dop.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ogp.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://vpe.hysaishi.cn

[D04] 删除元素
来源：http://sou.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eze.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dng.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pjs.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://pvd.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fdg.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wrv.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ttn.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bqm.daria6918.cn

[D05] 访问与修改元素
来源：http://eay.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://csl.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zab.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lzw.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://clc.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://gzh.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://mxq.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rur.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zrh.epnwcf.com

[D06] 数组长度
来源：http://dsb.tian-w.cn

Py:   len(arr)
来源：http://dub.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://eev.fanxiaobao.xyz

JS:   arr.length
来源：http://shz.nanxuanxn.top

TS:   arr.length
来源：http://ubx.yfazqb.com

Java: list.size();
来源：http://aeb.fehbvm.com

Go:   len(arr)
来源：http://jgx.jianghu66.top

Ruby: arr.length; arr.size
来源：http://rdh.svipenyu.cn

C#:   list.Count;
来源：http://mgj.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://ric.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kvm.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://iba.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://fxx.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://bfk.sweek.top

Java: list.subList(1, 4);
来源：http://gvt.fzhhl.top

Go:   arr[1:4]
来源：http://tpg.cucudq.cn

Ruby: arr[1, 3]
来源：http://wmm.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://rpi.bbcook.cn

[D08] 合并两个数组
来源：http://ifo.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://vrv.ivvv.top

PHP:  array_merge($a, $b);
来源：http://uge.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gvq.316326.xyz

TS:   [...a, ...b];
来源：http://qjh.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yul.jqgufenzy.top

Go:   append(a, b...)
来源：http://ghu.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://jhj.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://qyz.andypj.xyz

[D09] 排序（升序）
来源：http://oda.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://bjd.hysaishi.cn

PHP:  sort($arr);
来源：http://yev.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cvf.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gju.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iav.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://twj.jinqigufen.top

Ruby: arr.sort
来源：http://jrc.shanyushiyangtech.top

C#:   list.Sort();
来源：http://qjl.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dxh.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vja.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uty.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfa.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jbv.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ucy.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ijc.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cjk.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nci.dashuyun.cn

[D11] 反转数组
来源：http://iid.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ydy.redwolf501.top

PHP:  array_reverse($arr);
来源：http://dyo.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bta.jinqigufen.top

TS:   [...arr].reverse();
来源：http://asi.bbcook.cn

Java: Collections.reverse(list);
来源：http://zyq.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://bfm.wangshuangyany.cn

Ruby: arr.reverse
来源：http://hrs.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://xrc.yvedp.cn

[D12] 查找元素下标
来源：http://yyy.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://azd.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xve.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iaz.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dys.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yeo.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://jyz.cqqwz.cn

Ruby: arr.index(x)
来源：http://ggv.yj202588.top

C#:   list.IndexOf(x);
来源：http://yiu.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://der.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kur.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zeu.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://gfs.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://abt.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwo.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ovm.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://nwr.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dyd.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://qmm.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogu.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gsj.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://qmr.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://yyc.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jen.fehbvm.com

Go:   // 手写循环
来源：http://dip.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://bgb.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://smf.yueranfly.top

[D15] 去重
来源：http://xfw.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mii.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://cop.sweek.top

JS:   [...new Set(arr)]
来源：http://xds.yfazqb.com

TS:   [...new Set(arr)]
来源：http://wen.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lzr.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://gix.cheryme.top

Ruby: arr.uniq
来源：http://xyh.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://fkg.gaohongyu789.top

[D16] 求和与平均值
来源：http://pgy.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fpi.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hmb.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oan.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gor.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgp.cashguo.top

Go:   // 手写循环累加
来源：http://nio.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vnq.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://jtr.tian-w.cn

[D17] 最大值与最小值
来源：http://pny.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://vbg.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://cie.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://olv.guannengcc.top

TS:   Math.max(...arr);
来源：http://uwj.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nuk.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jee.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://tfp.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://rgt.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://aai.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fxt.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://ubh.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nvn.chenzaomai.com

TS:   nested.flat();
来源：http://ccc.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xiv.pycfn.com

Go:   // 手写双层循环
来源：http://heg.9152youxi.cn

Ruby: nested.flatten
来源：http://jka.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://egc.zhengqikj.top

[D19] 按字段分组
来源：http://pxf.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ojn.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cii.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bdz.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rzr.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lbr.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://iss.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dcu.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mec.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://vft.zycfv.cn

Py:   Counter(arr)
来源：http://zik.havefunace.top

PHP:  array_count_values($arr);
来源：http://sru.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://her.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfw.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bdm.cucudq.cn

Go:   // 手写 map[T]int
来源：http://mff.cashguo.top

Ruby: arr.tally
来源：http://mcn.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ehw.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://ncb.tianlin.xyz

Py:   x in arr
来源：http://amk.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://bor.c1oappe.top

JS:   arr.includes(x)
来源：http://ein.ctjpmb.com

TS:   arr.includes(x)
来源：http://hab.jqgufenzy.top

Java: list.contains(x)
来源：http://frj.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://pmd.c1oappe.top

Ruby: arr.include?(x)
来源：http://cnt.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://zrw.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://gex.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hvu.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fml.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://idb.birdmap.top

TS:   [...arr];
来源：http://fdw.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://ezk.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cyl.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://ceb.andypj.xyz

C#:   new List<int>(list);
来源：http://gdk.yuanzhike.top

[D23] reduce 累积计算
来源：http://ret.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pba.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wmg.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwh.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eta.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://unp.sjlbkw.cn

Go:   // 手写循环
来源：http://tgg.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aek.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ixi.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://ayv.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lfq.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rnf.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gov.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://guj.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vwg.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zkr.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qfu.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xrw.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://ior.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iyl.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tkj.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sqb.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hzn.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tkm.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wab.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zlb.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iwu.cdnleiting.top

[D26] 数组转字符串
来源：http://fcp.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://hqc.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://qov.jianghu66.top

JS:   arr.join(", ")
来源：http://snf.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://lzs.zhijiandao.cn

Java: String.join(", ", list)
来源：http://ojh.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://odk.havefunace.top

Ruby: arr.join(", ")
来源：http://uso.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://bqs.yj20258.top

================================================================================
来源：http://mah.hongshengwenyu.top

E. 字符串处理
来源：http://gug.ivvv.top

================================================================================
来源：http://qob.hesvh.cn

[E01] 拼接字符串
来源：http://sep.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kab.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zkh.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uhe.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://izr.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nwd.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://czy.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lym.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xaw.hesvh.cn

[E02] 重复字符串
来源：http://qry.sjlbkw.cn

Py:   "ab" * 3
来源：http://iwf.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://zol.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://wtu.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://qpe.chenlongwang.top

Java: "ab".repeat(3)
来源：http://zcg.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://ait.gogol.net.cn

Ruby: "ab" * 3
来源：http://rau.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nck.snrcjt.cn

[E03] 截取子串
来源：http://jtu.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vxb.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tww.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bdm.fehbvm.com

TS:   s.slice(1, 4)
来源：http://kqg.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://vqp.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://brv.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://psf.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://vql.sweek.top

[E04] 查找子串位置
来源：http://bep.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://ryg.cashguo.top

PHP:  strpos($s, "x");
来源：http://mvw.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://spu.hfpthk.cn

TS:   s.indexOf("x")
来源：http://lbb.jinqigufen.top

Java: s.indexOf("x")
来源：http://brp.jinqigfzy.top


<!-- 参考信息 -->