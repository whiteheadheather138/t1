代发 wailian999

[C14] 泛型函数
来源：http://rjm.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tzt.jqgufenzy.top

PHP:  // 无泛型
来源：http://vkz.iojbl.cn

JS:   // 无泛型
来源：http://usq.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://onz.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jsg.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgu.hnxiangtu.top

Ruby: # 无泛型
来源：http://olq.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bdc.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://zdt.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jzu.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://zhn.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udq.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ucn.aizwys.cn

Java: // 无解构
来源：http://yac.chenjidiqi.icu

Go:   // 无解构
来源：http://wdd.zhengqikj.top

Ruby: a, b = pair
来源：http://lnl.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://fww.wangdashe.top

[C16] 函数 / 方法重载
来源：http://ltr.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rob.iojbl.cn

PHP:  // 无重载
来源：http://qny.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ghq.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://twy.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ysd.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://hsj.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://mdz.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qhq.meibo888.top

================================================================================
来源：http://ojp.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://fyn.meibo888.top

================================================================================
来源：http://rgj.yj202588.top

[D01] 创建数组 / 列表
来源：http://ihw.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gvo.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kan.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qvi.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dty.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cnt.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://djy.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://mwr.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fzr.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://sby.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yxv.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://grc.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://rkx.snrcjt.cn

TS:   arr.push(4);
来源：http://itz.meibo888.top

Java: list.add(4);
来源：http://acu.meibo888.top

Go:   arr = append(arr, 4)
来源：http://tig.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://mfj.andypj.xyz

C#:   list.Add(4);
来源：http://sgg.havefunace.top

[D03] 在指定位置插入元素
来源：http://vhs.pycfn.com

Py:   arr.insert(0, 0)
来源：http://yre.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pay.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zvs.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://xne.bjfxy.top

Java: list.add(0, 0);
来源：http://ncc.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://npb.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://syq.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://mhz.snrcjt.cn

[D04] 删除元素
来源：http://kch.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bvd.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bha.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lse.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://wmq.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://krc.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mak.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aoj.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://svd.hnqzz.top

[D05] 访问与修改元素
来源：http://ofy.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pze.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vgn.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fjr.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://krm.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://fla.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://qbp.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wyx.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxu.sufxvd.cn

[D06] 数组长度
来源：http://ecr.iojbl.cn

Py:   len(arr)
来源：http://ovk.ehwqpu.com

PHP:  count($arr);
来源：http://ila.mhx1999.top

JS:   arr.length
来源：http://ngb.jqgufenzy.top

TS:   arr.length
来源：http://wuw.hcnkem.com

Java: list.size();
来源：http://urx.0kj1m.cn

Go:   len(arr)
来源：http://iwr.tarul.cn

Ruby: arr.length; arr.size
来源：http://ojv.daxiang520.top

C#:   list.Count;
来源：http://vxl.birdmap.top

[D07] 切片 / 取子数组
来源：http://qjy.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxt.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qcg.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://tse.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://gdf.zdbjq.cn

Java: list.subList(1, 4);
来源：http://gsx.jlsjyb.cn

Go:   arr[1:4]
来源：http://cxb.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://qun.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://elw.tanke756.top

[D08] 合并两个数组
来源：http://rxj.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://eof.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://tpw.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bnm.gzhubu.top

TS:   [...a, ...b];
来源：http://awj.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iel.yonumen.top

Go:   append(a, b...)
来源：http://mkb.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://vlv.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://mdb.birdmap.top

[D09] 排序（升序）
来源：http://xzy.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://jix.yuanzhike.top

PHP:  sort($arr);
来源：http://ksf.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kwf.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://nid.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mop.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vjd.sysykeji.top

Ruby: arr.sort
来源：http://lhj.vehdjk.com

C#:   list.Sort();
来源：http://jun.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fcv.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uau.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwz.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsu.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahx.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://apu.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lbo.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gsa.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kje.yangfankeji.com

[D11] 反转数组
来源：http://fwf.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://zcz.zycfv.cn

PHP:  array_reverse($arr);
来源：http://vzs.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zbn.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://xef.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://rkw.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://bqo.hongshengwenyu.top

Ruby: arr.reverse
来源：http://ocj.cheryme.top

C#:   list.Reverse();
来源：http://zhn.havefunace.top

[D12] 查找元素下标
来源：http://rif.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://fvk.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qdb.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfm.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdx.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yps.hammf.cn

Go:   slices.Index(arr, x)
来源：http://tsd.bbcook.cn

Ruby: arr.index(x)
来源：http://wnc.jianghu66.top

C#:   list.IndexOf(x);
来源：http://yne.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://mrx.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mgy.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wqv.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://tqe.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://szb.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://luq.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xzl.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nyl.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://phd.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://gtf.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xoe.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vao.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://uox.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://lcl.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bdx.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://okc.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://nrk.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://adv.uphjek.com

[D15] 去重
来源：http://bhw.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kiq.cucudq.cn

PHP:  array_unique($arr);
来源：http://xsj.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://okd.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://bzj.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yfl.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://qka.cashguo.top

Ruby: arr.uniq
来源：http://fbw.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://frl.jianghu66.top

[D16] 求和与平均值
来源：http://bym.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sze.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hrb.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vif.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kbs.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zja.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://kyy.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vpd.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://tph.yfazqb.com

[D17] 最大值与最小值
来源：http://wax.sweek.top

Py:   max(arr);  min(arr)
来源：http://iht.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://aar.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xyi.shuidangran.top

TS:   Math.max(...arr);
来源：http://nak.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aeu.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lpa.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://seu.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://sva.yonumen.top

[D18] 扁平化嵌套数组
来源：http://wum.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hli.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://pal.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xgn.316326.xyz

TS:   nested.flat();
来源：http://ilj.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jsz.hnxiangtu.top

Go:   // 手写双层循环
来源：http://owg.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://ewz.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fmg.fanxiaobao.xyz

[D19] 按字段分组
来源：http://kyw.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hoq.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fed.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rah.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cuj.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wte.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://sjg.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jzz.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eit.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://qjk.gotoacloud.top

Py:   Counter(arr)
来源：http://yft.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://luw.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qfs.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kwz.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ldh.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://ugk.tanke756.top

Ruby: arr.tally
来源：http://ifg.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://orc.hnqzz.top

[D21] 判断是否包含某元素
来源：http://neu.shanyushiyangkeji.top

Py:   x in arr
来源：http://ymv.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://tpj.guannengcc.top

JS:   arr.includes(x)
来源：http://ejy.havefunace.top

TS:   arr.includes(x)
来源：http://zoa.yongpay.top

Java: list.contains(x)
来源：http://msg.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://ien.yvedp.cn

Ruby: arr.include?(x)
来源：http://mbb.zhixingplan.top

C#:   list.Contains(x)
来源：http://hcl.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://ahd.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vxz.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://acp.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://brl.iojbl.cn

TS:   [...arr];
来源：http://yhh.fehbvm.com

Java: new ArrayList<>(list);
来源：http://ynb.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://zbk.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://hue.daria6918.cn

C#:   new List<int>(list);
来源：http://kvm.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://aej.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ggh.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vcw.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mak.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yos.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tjr.jinghuilouyu.cn

Go:   // 手写循环
来源：http://qux.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hlf.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sxw.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://nxl.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fnm.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dcj.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyk.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dhl.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zbp.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iup.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ubo.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ofq.hammf.cn

[D25] Set 集合去重与交并差
来源：http://nys.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eel.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohq.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ivy.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cpb.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ibu.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cls.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dcl.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gwa.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://cyp.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://teb.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://izd.sufxvd.cn

JS:   arr.join(", ")
来源：http://hum.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://blt.snrcjt.cn

Java: String.join(", ", list)
来源：http://biz.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://ynf.0kj1m.cn

Ruby: arr.join(", ")
来源：http://hio.yueranfly.top

C#:   string.Join(", ", list)
来源：http://txl.fktsv.cn

================================================================================
来源：http://nja.tarul.cn

E. 字符串处理
来源：http://tlr.chenlongwang.top

================================================================================
来源：http://cqm.yanxiufei.cn

[E01] 拼接字符串
来源：http://teb.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eux.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://api.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cev.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dna.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://whp.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ait.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xcj.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ykj.sufxvd.cn

[E02] 重复字符串
来源：http://ygj.snrcjt.cn

Py:   "ab" * 3
来源：http://zru.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://jhs.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://jyk.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://mpo.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://hvs.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://lqs.hnqzz.top

Ruby: "ab" * 3
来源：http://hsd.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://udj.mhx1999.top

[E03] 截取子串
来源：http://dhb.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hwj.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tal.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vwe.sweek.top

TS:   s.slice(1, 4)
来源：http://fkl.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://tzv.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dak.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://kqn.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://gqy.shangyingyoupin.top

[E04] 查找子串位置
来源：http://yuv.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://gze.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://xil.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cga.svipenyu.cn

TS:   s.indexOf("x")
来源：http://pmi.jinqigufen.top

Java: s.indexOf("x")
来源：http://kta.daria6918.cn


<!-- 参考信息 -->