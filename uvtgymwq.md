代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://leq.zhixingplan.top

Go:   func add(a, b int) int
来源：http://njf.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nqx.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://fko.jinqigufen.top

[C14] 泛型函数
来源：http://yfg.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hjy.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://bqo.dashuyun.cn

JS:   // 无泛型
来源：http://gvv.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bfq.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qpe.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xsp.zdqjudy.top

Ruby: # 无泛型
来源：http://ukc.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://djv.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://etn.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yoj.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://kzd.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nbc.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://alo.nwbrower.top

Java: // 无解构
来源：http://pjq.tanke756.top

Go:   // 无解构
来源：http://lng.nwbrower.top

Ruby: a, b = pair
来源：http://ftl.jianghu66.top

C#:   var (a, b) = pair;
来源：http://voo.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://qrd.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tdh.xinyue.icu

PHP:  // 无重载
来源：http://haj.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://chh.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://wok.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gwm.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://tfk.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://gvi.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ryo.dashuyun.cn

================================================================================
来源：http://wgm.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://tbc.vqdsnc.cn

================================================================================
来源：http://ali.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://vkt.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zst.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jao.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pxm.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rwh.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sjy.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://nni.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://rtk.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://glo.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://kwz.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bqt.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gdg.sysykeji.top

JS:   arr.push(4);
来源：http://wix.jianghu66.top

TS:   arr.push(4);
来源：http://ftf.hnxiangtu.top

Java: list.add(4);
来源：http://kkb.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://jss.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://ogm.cqqwz.cn

C#:   list.Add(4);
来源：http://hvu.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://meg.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://pzk.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ltv.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yrk.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://xka.ydzc1.top

Java: list.add(0, 0);
来源：http://xtm.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cye.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ray.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://zsy.yvedp.cn

[D04] 删除元素
来源：http://sij.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qag.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cuc.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dqg.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://adp.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmf.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vjm.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dca.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bug.cqqwz.cn

[D05] 访问与修改元素
来源：http://jlh.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xpx.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ijx.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ibb.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xaq.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://upv.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://ctt.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fyw.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://leo.yj20258.top

[D06] 数组长度
来源：http://hqk.0kj1m.cn

Py:   len(arr)
来源：http://jxz.daxiang520.top

PHP:  count($arr);
来源：http://xin.hnqzz.top

JS:   arr.length
来源：http://nni.hnqzz.top

TS:   arr.length
来源：http://avt.ydzc1.top

Java: list.size();
来源：http://jcu.0kj1m.cn

Go:   len(arr)
来源：http://vlq.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://zha.guannengcc.top

C#:   list.Count;
来源：http://xah.yvedp.cn

[D07] 切片 / 取子数组
来源：http://pao.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fxe.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jgj.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://uou.cheryme.top

TS:   arr.slice(1, 4);
来源：http://izv.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://ben.xziqi.cn

Go:   arr[1:4]
来源：http://mcl.mhx1999.top

Ruby: arr[1, 3]
来源：http://nja.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://vrc.ydzc1.top

[D08] 合并两个数组
来源：http://lny.sweek.top

Py:   a + b;  a.extend(b)
来源：http://lzd.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://ndf.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ljj.shuidangran.top

TS:   [...a, ...b];
来源：http://vkh.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iqh.yj20258888.top

Go:   append(a, b...)
来源：http://abb.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://mbg.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://bjg.dashuyun.cn

[D09] 排序（升序）
来源：http://iad.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://omk.daria6918.cn

PHP:  sort($arr);
来源：http://mcv.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://unq.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ncu.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fkx.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://str.gaohongyu789.top

Ruby: arr.sort
来源：http://qma.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://vub.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kmw.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://urb.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iui.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yon.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fph.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gjt.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vup.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lbj.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yvs.zdqjudy.top

[D11] 反转数组
来源：http://hbk.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://dxd.c1oappe.top

PHP:  array_reverse($arr);
来源：http://sbs.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lhw.sweek.top

TS:   [...arr].reverse();
来源：http://iij.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://pil.ivvv.top

Go:   slices.Reverse(arr)
来源：http://ujk.sysykeji.top

Ruby: arr.reverse
来源：http://oct.tanke756.top

C#:   list.Reverse();
来源：http://mak.guannengcc.top

[D12] 查找元素下标
来源：http://uby.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://hsy.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qps.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mek.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldw.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://due.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://eyk.yueranfly.top

Ruby: arr.index(x)
来源：http://kia.gzhubu.top

C#:   list.IndexOf(x);
来源：http://zpg.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://bvs.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jmt.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ixi.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://cdn.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://yll.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://szx.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tqb.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hck.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nig.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://hgr.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cty.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lss.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://hdl.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://uaw.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xab.hcnkem.com

Go:   // 手写循环
来源：http://mgs.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://mgr.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hwe.sysykeji.top

[D15] 去重
来源：http://woa.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://exx.ivvv.top

PHP:  array_unique($arr);
来源：http://xwa.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://ler.bjfxy.top

TS:   [...new Set(arr)]
来源：http://wqr.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sym.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://gdg.jinqigfzy.top

Ruby: arr.uniq
来源：http://foy.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://xyu.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://xja.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://srb.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bwb.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://auh.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dyn.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hpw.jianghu66.top

Go:   // 手写循环累加
来源：http://lrz.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://van.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://noy.zhixingplan.top

[D17] 最大值与最小值
来源：http://leu.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://xzt.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://hjf.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rwh.fktsv.cn

TS:   Math.max(...arr);
来源：http://xbd.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jxw.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eui.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://plg.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://fcp.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://oxb.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wkp.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://rvx.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zcq.guowangkeji.top

TS:   nested.flat();
来源：http://rgz.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lvo.zycfv.cn

Go:   // 手写双层循环
来源：http://gsg.hcnkem.com

Ruby: nested.flatten
来源：http://rqs.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eot.yueranfly.top

[D19] 按字段分组
来源：http://gje.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pde.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kkg.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qfn.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sgq.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mvp.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://fzr.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zzy.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zpw.hammf.cn

[D20] 统计每个元素出现次数
来源：http://hvf.ctjpmb.com

Py:   Counter(arr)
来源：http://mbr.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://wve.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kms.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bfc.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eja.tanke756.top

Go:   // 手写 map[T]int
来源：http://euf.xinyue.icu

Ruby: arr.tally
来源：http://pgi.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aou.sysykeji.top

[D21] 判断是否包含某元素
来源：http://xrg.aibaodan.cn

Py:   x in arr
来源：http://ulz.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://qtg.gaohongyu789.top

JS:   arr.includes(x)
来源：http://mpw.birdmap.top

TS:   arr.includes(x)
来源：http://klz.birdmap.top

Java: list.contains(x)
来源：http://ifx.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://yvw.zdqjudy.top

Ruby: arr.include?(x)
来源：http://kak.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://xyi.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://dnz.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://foi.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wwr.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ycc.hfpthk.cn

TS:   [...arr];
来源：http://kfr.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://oxw.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://pwr.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://bqx.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://dmo.ybcxt.top

[D23] reduce 累积计算
来源：http://npk.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sxj.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xfk.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qcb.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fdv.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://men.xinyue.icu

Go:   // 手写循环
来源：http://jrq.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nny.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rmu.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://xwz.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tgq.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rzb.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfy.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vzw.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://twx.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uyb.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aaa.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ohk.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://zny.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jtv.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ckz.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qhr.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://abg.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://djv.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://igq.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://exy.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://duq.dashuyun.cn

[D26] 数组转字符串
来源：http://tyn.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://wwr.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://gfv.zhongyouzk.top

JS:   arr.join(", ")
来源：http://ary.fengsongda.top

TS:   arr.join(", ")
来源：http://jvb.zhoulong.xyz

Java: String.join(", ", list)
来源：http://mdv.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://eod.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://tmh.havefunace.top

C#:   string.Join(", ", list)
来源：http://syl.fktsv.cn

================================================================================
来源：http://omk.quarkkingdee.top

E. 字符串处理
来源：http://rhv.zhixingplan.top

================================================================================
来源：http://qxi.dashuyun.cn

[E01] 拼接字符串
来源：http://gze.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://trw.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kud.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gul.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://knn.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uev.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvm.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eim.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yku.yueranfly.top

[E02] 重复字符串
来源：http://blu.yongpay.top

Py:   "ab" * 3
来源：http://bbn.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://scm.cashguo.top

JS:   "ab".repeat(3)
来源：http://stz.hesvh.cn

TS:   "ab".repeat(3)
来源：http://ycj.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://rkx.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://dph.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://mmp.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fwq.jinqigfzy.top

[E03] 截取子串
来源：http://khp.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dsb.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jdk.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oad.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://etm.fehbvm.com

Java: s.substring(1, 4)
来源：http://bgy.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wqm.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://mxy.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://icj.bbcook.cn

[E04] 查找子串位置
来源：http://xjn.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://aox.zhongyouzk.top


<!-- 参考信息 -->