代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://zfp.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://nfq.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fgh.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mrc.svipenyu.cn

[C14] 泛型函数
来源：http://zxs.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rgb.zhengqikj.top

PHP:  // 无泛型
来源：http://lrv.chenzaomai.com

JS:   // 无泛型
来源：http://rst.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blb.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bpq.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sfs.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://uba.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ueh.yongpay.top

[C15] 解构 / 展开参数
来源：http://wkj.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bli.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://lfz.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fbi.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rip.tian-w.cn

Java: // 无解构
来源：http://gkd.zhaomingkeji.xyz

Go:   // 无解构
来源：http://wlu.ppjwa.cn

Ruby: a, b = pair
来源：http://ivx.fehbvm.com

C#:   var (a, b) = pair;
来源：http://jxd.iojbl.cn

[C16] 函数 / 方法重载
来源：http://pro.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bgf.ivvv.top

PHP:  // 无重载
来源：http://pzz.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iqx.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://sbe.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://yct.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://xtl.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://mcf.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dug.zhiwuduotai.top

================================================================================
来源：http://lxv.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://spp.yj202588.top

================================================================================
来源：http://hkm.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://wjy.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oad.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zrj.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ytc.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kuw.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pxd.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://kwu.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://gzh.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jst.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://ocw.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dxu.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cto.zdbjq.cn

JS:   arr.push(4);
来源：http://esa.cqqwz.cn

TS:   arr.push(4);
来源：http://lvj.hfpthk.cn

Java: list.add(4);
来源：http://svh.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://mbd.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://gcu.tanke756.top

C#:   list.Add(4);
来源：http://eyk.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://eka.hammf.cn

Py:   arr.insert(0, 0)
来源：http://ile.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tje.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wqq.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://mln.tanke756.top

Java: list.add(0, 0);
来源：http://rpm.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://oco.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://crt.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://drr.gogol.net.cn

[D04] 删除元素
来源：http://mjk.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sbn.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nqc.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mhj.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://qmp.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qfv.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pau.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tjt.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nou.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://ozp.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xnu.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tox.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dcz.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://nju.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://cek.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://ple.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zkp.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xuj.hywenlv.cn

[D06] 数组长度
来源：http://pga.guowangkeji.top

Py:   len(arr)
来源：http://duf.yuxming.cn

PHP:  count($arr);
来源：http://xsa.feifeiyinyue.top

JS:   arr.length
来源：http://ubq.cqqwz.cn

TS:   arr.length
来源：http://rux.pycfn.com

Java: list.size();
来源：http://dix.zdqjudy.top

Go:   len(arr)
来源：http://mcr.316326.xyz

Ruby: arr.length; arr.size
来源：http://uuk.hcnkem.com

C#:   list.Count;
来源：http://dsq.tarul.cn

[D07] 切片 / 取子数组
来源：http://dce.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ffg.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://bwz.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://lpl.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://yvj.yongpay.top

Java: list.subList(1, 4);
来源：http://gqx.zdbjq.cn

Go:   arr[1:4]
来源：http://tbm.hysaishi.cn

Ruby: arr[1, 3]
来源：http://jdt.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://jtt.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://fwc.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://cyx.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://bfw.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gph.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://bok.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ujw.fengsongda.top

Go:   append(a, b...)
来源：http://pfm.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://axc.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://ngk.gotoacloud.top

[D09] 排序（升序）
来源：http://gxx.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://nky.cucudq.cn

PHP:  sort($arr);
来源：http://xog.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rbp.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pmg.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sle.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hkr.havefunace.top

Ruby: arr.sort
来源：http://pml.chenlongwang.top

C#:   list.Sort();
来源：http://djl.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://hpl.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xga.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cio.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hce.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgi.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ons.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zov.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vgb.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cca.zhoulong.xyz

[D11] 反转数组
来源：http://rpu.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zon.yueranfly.top

PHP:  array_reverse($arr);
来源：http://oue.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wmp.iojbl.cn

TS:   [...arr].reverse();
来源：http://tna.0kj1m.cn

Java: Collections.reverse(list);
来源：http://byr.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://iro.chenzaomai.com

Ruby: arr.reverse
来源：http://ppz.daria6918.cn

C#:   list.Reverse();
来源：http://msn.hesvh.cn

[D12] 查找元素下标
来源：http://hrm.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://urm.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pvw.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mqb.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dax.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qvp.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://zkc.yueranfly.top

Ruby: arr.index(x)
来源：http://sir.yj20258888.top

C#:   list.IndexOf(x);
来源：http://bhl.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://izf.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cbt.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://chv.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://glx.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://jgr.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aie.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xot.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://xml.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ztm.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://hvd.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dtg.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bqs.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://tyb.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://sle.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rvo.chenlongwang.top

Go:   // 手写循环
来源：http://tei.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://lvq.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xvk.fehbvm.com

[D15] 去重
来源：http://xmb.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cxz.nwbrower.top

PHP:  array_unique($arr);
来源：http://lur.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://phv.cucudq.cn

TS:   [...new Set(arr)]
来源：http://ynl.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wwc.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://kcn.hnqzz.top

Ruby: arr.uniq
来源：http://nvq.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://odk.bbcook.cn

[D16] 求和与平均值
来源：http://glj.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfd.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hhq.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://trk.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ckz.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qeg.zhijiandao.cn

Go:   // 手写循环累加
来源：http://fra.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qfp.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://dcg.ctjpmb.com

[D17] 最大值与最小值
来源：http://bas.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://crf.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://slk.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://opd.zycfv.cn

TS:   Math.max(...arr);
来源：http://dnt.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ayb.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxa.yonumen.top

Ruby: arr.max;  arr.min
来源：http://ype.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://pvb.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://apm.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lup.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://woh.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ljw.zhongyouzk.top

TS:   nested.flat();
来源：http://njv.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uqf.hnxiangtu.top

Go:   // 手写双层循环
来源：http://fku.shuidangran.top

Ruby: nested.flatten
来源：http://iog.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wvv.meibo888.top

[D19] 按字段分组
来源：http://xve.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lyr.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lks.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ltb.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vez.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aiv.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://qma.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vyf.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://srb.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://koz.ctjpmb.com

Py:   Counter(arr)
来源：http://gvr.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://fhd.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fiz.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hnr.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ers.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://ice.havefunace.top

Ruby: arr.tally
来源：http://daw.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hyq.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://shw.ppjwa.cn

Py:   x in arr
来源：http://zqq.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://rvs.zdbjq.cn

JS:   arr.includes(x)
来源：http://sys.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://pzz.yvedp.cn

Java: list.contains(x)
来源：http://vjd.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://jrd.ydzc1.top

Ruby: arr.include?(x)
来源：http://wwj.ppjwa.cn

C#:   list.Contains(x)
来源：http://yvj.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://uxr.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://huc.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oix.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wny.fehbvm.com

TS:   [...arr];
来源：http://fca.tarul.cn

Java: new ArrayList<>(list);
来源：http://enj.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://mvn.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://uxm.kuanghao11.cn

C#:   new List<int>(list);
来源：http://ahp.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://mqq.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uvy.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oaj.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yel.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vfb.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qqo.ydzc1.top

Go:   // 手写循环
来源：http://fbz.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tvs.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zzs.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://bbz.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lxj.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ocu.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rht.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mmy.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mvo.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nff.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://prk.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rpt.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://sli.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aae.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ghn.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vjp.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jxq.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://znp.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ypp.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wmk.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qhj.tianlin.xyz

[D26] 数组转字符串
来源：http://chh.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://gds.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://nps.chenlongwang.top

JS:   arr.join(", ")
来源：http://myi.zhongyouzk.top

TS:   arr.join(", ")
来源：http://baw.zdbjq.cn

Java: String.join(", ", list)
来源：http://iis.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://dva.chenzaomai.com

Ruby: arr.join(", ")
来源：http://eaf.yj20258888.top

C#:   string.Join(", ", list)
来源：http://mpq.zdbjq.cn

================================================================================
来源：http://acn.cqqwz.cn

E. 字符串处理
来源：http://pig.zhoulong.xyz

================================================================================
来源：http://mao.hywenlv.cn

[E01] 拼接字符串
来源：http://nlm.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fjc.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://moc.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tur.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jta.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzd.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jxd.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wke.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gqn.shangyingyoupin.top

[E02] 重复字符串
来源：http://cev.aizwys.cn

Py:   "ab" * 3
来源：http://ayi.daria6918.cn

PHP:  str_repeat("ab", 3);
来源：http://pkd.fzhhl.top

JS:   "ab".repeat(3)
来源：http://mcq.yfazqb.com

TS:   "ab".repeat(3)
来源：http://lvw.birdmap.top

Java: "ab".repeat(3)
来源：http://jxy.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://bcs.sysykeji.top

Ruby: "ab" * 3
来源：http://ykv.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ptv.316326.xyz

[E03] 截取子串
来源：http://yvp.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://itn.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://peg.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qbq.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://ypb.vehdjk.com

Java: s.substring(1, 4)
来源：http://txj.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nil.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://flb.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://atn.pengpengdd.cyou

[E04] 查找子串位置
来源：http://ryx.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://evv.meibo888.top


<!-- 参考信息 -->