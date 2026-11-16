代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://dbz.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://lkx.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://gnm.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://buz.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://hgk.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://ify.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kxv.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://sej.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hoe.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yua.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rjk.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcf.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lvg.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://gqg.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hbw.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://igb.fanxiaobao.xyz

[C14] 泛型函数
来源：http://jqc.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pig.jiagoushi.top

PHP:  // 无泛型
来源：http://itr.yueranfly.top

JS:   // 无泛型
来源：http://zku.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://snc.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lqa.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vav.tarul.cn

Ruby: # 无泛型
来源：http://xne.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ixt.wangdashe.top

[C15] 解构 / 展开参数
来源：http://zvy.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fgt.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://ayr.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://skw.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jxx.hywenlv.cn

Java: // 无解构
来源：http://myt.yanxiufei.cn

Go:   // 无解构
来源：http://zhb.hesvh.cn

Ruby: a, b = pair
来源：http://ghu.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://ytm.aizwys.cn

[C16] 函数 / 方法重载
来源：http://dkq.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wik.andypj.xyz

PHP:  // 无重载
来源：http://qhg.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://djx.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://ykj.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wgv.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://nsv.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://dpv.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hmm.yj20258.top

================================================================================
来源：http://zxs.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://zje.52xcode.cn

================================================================================
来源：http://nnz.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://kik.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ddb.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jzj.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uyg.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wsj.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kmw.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://orc.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://oyk.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wuo.0kj1m.cn

[D02] 追加元素到末尾
来源：http://uju.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hgt.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uhr.tianlin.xyz

JS:   arr.push(4);
来源：http://vcl.yanxiufei.cn

TS:   arr.push(4);
来源：http://yog.yj202588.top

Java: list.add(4);
来源：http://cvq.cashguo.top

Go:   arr = append(arr, 4)
来源：http://zqi.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://tuz.dianchejie.cn

C#:   list.Add(4);
来源：http://xon.aizwys.cn

[D03] 在指定位置插入元素
来源：http://uka.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://kxi.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hcj.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bij.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://eil.chenlongwang.top

Java: list.add(0, 0);
来源：http://vmm.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://jte.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gpz.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://ivz.vehdjk.com

[D04] 删除元素
来源：http://nsb.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://klq.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvn.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pnu.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://iiz.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nhh.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jcr.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xth.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pyz.316326.xyz

[D05] 访问与修改元素
来源：http://wlm.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://elq.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uzx.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nki.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://bsp.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://dsi.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://gga.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gyh.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fpy.jinqigufen.top

[D06] 数组长度
来源：http://nmm.vqdsnc.cn

Py:   len(arr)
来源：http://wco.xuanzx.com

PHP:  count($arr);
来源：http://nzn.zdqjudy.top

JS:   arr.length
来源：http://len.hysaishi.cn

TS:   arr.length
来源：http://pys.andypj.xyz

Java: list.size();
来源：http://des.xuetiantiany.cn

Go:   len(arr)
来源：http://pte.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://hyu.daxiang520.top

C#:   list.Count;
来源：http://oxd.wangdashe.top

[D07] 切片 / 取子数组
来源：http://cga.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zog.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gwu.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://rnw.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://qku.xziqi.cn

Java: list.subList(1, 4);
来源：http://ziz.svipenyu.cn

Go:   arr[1:4]
来源：http://kbn.yj20258888.top

Ruby: arr[1, 3]
来源：http://jro.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://asc.andypj.xyz

[D08] 合并两个数组
来源：http://vql.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://bbx.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://khb.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nsy.wangdashe.top

TS:   [...a, ...b];
来源：http://ees.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://elh.bbcook.cn

Go:   append(a, b...)
来源：http://cox.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://pwz.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://bhc.mhx1999.top

[D09] 排序（升序）
来源：http://hnl.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://jbg.jqgfzy.top

PHP:  sort($arr);
来源：http://aqz.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vmw.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bzz.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ymi.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nly.bbcook.cn

Ruby: arr.sort
来源：http://tqh.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://waf.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://ngf.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgr.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iid.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngy.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ott.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://evf.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://trk.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hur.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mqv.bbcook.cn

[D11] 反转数组
来源：http://ndj.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fau.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://gjm.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hnf.redwolf501.top

TS:   [...arr].reverse();
来源：http://ews.jyoumei.cn

Java: Collections.reverse(list);
来源：http://pxq.sweek.top

Go:   slices.Reverse(arr)
来源：http://zyn.fehbvm.com

Ruby: arr.reverse
来源：http://lkb.fengsongda.top

C#:   list.Reverse();
来源：http://lli.uphjek.com

[D12] 查找元素下标
来源：http://mlb.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://oop.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://evy.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqa.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cst.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://woz.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://exc.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://rfh.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://zrv.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://pxu.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cos.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pna.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://hmx.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://rww.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gib.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hpo.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://yac.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://apo.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://ccs.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://czy.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wig.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://wcy.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://mmi.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://wvk.pengpengdd.cyou

Go:   // 手写循环
来源：http://drk.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://joc.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ptg.yuxming.cn

[D15] 去重
来源：http://zng.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jtn.yueranfly.top

PHP:  array_unique($arr);
来源：http://imm.xylfe.cn

JS:   [...new Set(arr)]
来源：http://dzj.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://ldv.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dnu.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lsu.cashguo.top

Ruby: arr.uniq
来源：http://rem.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://heq.nanxinkj.top

[D16] 求和与平均值
来源：http://zlo.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghv.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emf.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://epi.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://itl.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aob.daria6918.cn

Go:   // 手写循环累加
来源：http://usq.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hsj.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://vel.aizwys.cn

[D17] 最大值与最小值
来源：http://sgj.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://fgt.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://szk.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wek.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://sak.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://sda.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://krg.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://mft.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://cdn.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://vla.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://klu.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://zrt.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ckz.sweek.top

TS:   nested.flat();
来源：http://ahj.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ufi.hammf.cn

Go:   // 手写双层循环
来源：http://fxp.dashuyun.cn

Ruby: nested.flatten
来源：http://vir.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vbg.cdnleiting.top

[D19] 按字段分组
来源：http://sej.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xzl.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wki.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iah.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ali.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://com.meibo888.top

Go:   // 手写 map[string][]T
来源：http://xnb.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yaw.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyd.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://rhr.chenlongwang.top

Py:   Counter(arr)
来源：http://mlz.yvedp.cn

PHP:  array_count_values($arr);
来源：http://nrk.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwp.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lvu.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arp.fzhhl.top

Go:   // 手写 map[T]int
来源：http://iev.tian-w.cn

Ruby: arr.tally
来源：http://ajm.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uzn.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://iuh.havefunace.top

Py:   x in arr
来源：http://xow.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://yob.hcnkem.com

JS:   arr.includes(x)
来源：http://sfu.svipenyu.cn

TS:   arr.includes(x)
来源：http://xnc.yfazqb.com

Java: list.contains(x)
来源：http://nay.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://drs.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://awl.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://fas.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://tzk.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjb.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qdx.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qth.jinqigfzy.top

TS:   [...arr];
来源：http://sgp.iojbl.cn

Java: new ArrayList<>(list);
来源：http://vki.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://ofs.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://vec.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://ggg.birdmap.top

[D23] reduce 累积计算
来源：http://ihv.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xql.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://usc.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipt.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxk.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ndj.chenzaomai.com

Go:   // 手写循环
来源：http://xfl.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hul.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ytg.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://kmc.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kzc.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gve.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eer.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yxp.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://npc.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jdr.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://elb.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vqf.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://nvn.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xkq.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bow.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ovv.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vvq.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hlu.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mjz.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xcv.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kbq.jyoumei.cn

[D26] 数组转字符串
来源：http://tys.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://fxq.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://iev.vqdsnc.cn

JS:   arr.join(", ")
来源：http://pqj.ehwqpu.com

TS:   arr.join(", ")
来源：http://bno.vqdsnc.cn

Java: String.join(", ", list)
来源：http://sxr.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://ypl.yuanzhike.top

Ruby: arr.join(", ")
来源：http://gya.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://ikh.gogol.net.cn

================================================================================
来源：http://nal.ctjpmb.com

E. 字符串处理
来源：http://ybh.yueranfly.top

================================================================================
来源：http://pyy.vehdjk.com

[E01] 拼接字符串
来源：http://cfd.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cbe.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ayk.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wus.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqh.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ogw.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tht.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vrn.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kqo.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://nsi.daria6918.cn

Py:   "ab" * 3
来源：http://icu.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://oiq.daxiang520.top

JS:   "ab".repeat(3)
来源：http://qgb.epnwcf.com

TS:   "ab".repeat(3)
来源：http://rjp.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://obr.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://uhm.sufxvd.cn

Ruby: "ab" * 3
来源：http://zmw.yangfankeji.com


<!-- 参考信息 -->