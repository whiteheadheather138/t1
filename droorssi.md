代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://htv.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://hsz.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://sfb.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fan.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://hvs.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://pto.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://trw.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://iue.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xyc.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syo.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fcq.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdv.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bzn.yvedp.cn

Go:   func add(a, b int) int
来源：http://fyo.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cpp.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://eac.sweek.top

[C14] 泛型函数
来源：http://yrg.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xtv.ppjwa.cn

PHP:  // 无泛型
来源：http://arv.fehbvm.com

JS:   // 无泛型
来源：http://kyr.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xgi.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://had.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xzv.vqdsnc.cn

Ruby: # 无泛型
来源：http://tal.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlx.daxiang520.top

[C15] 解构 / 展开参数
来源：http://vbm.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pyc.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://cne.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zey.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kfe.wangdashe.top

Java: // 无解构
来源：http://stc.ydjk.org.cn

Go:   // 无解构
来源：http://bjf.cdnleiting.top

Ruby: a, b = pair
来源：http://svp.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://vnu.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://iwc.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xgd.yuanzhike.top

PHP:  // 无重载
来源：http://hso.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iha.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://ddv.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mww.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://mgp.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://zxc.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vqf.shanyushiyangkeji.top

================================================================================
来源：http://uvj.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://zee.xylfe.cn

================================================================================
来源：http://tvu.birdmap.top

[D01] 创建数组 / 列表
来源：http://snb.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nli.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tqs.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yrl.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://zho.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://opy.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://dqc.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://syf.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xpg.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://zgh.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yer.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rje.nwbrower.top

JS:   arr.push(4);
来源：http://ews.yj20258888.top

TS:   arr.push(4);
来源：http://lbm.yuanzhike.top

Java: list.add(4);
来源：http://zvy.hammf.cn

Go:   arr = append(arr, 4)
来源：http://dop.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://dld.andypj.xyz

C#:   list.Add(4);
来源：http://ziq.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://mhs.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://wym.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lbo.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://krf.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://xsh.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://edk.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://duc.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://thl.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://zwt.yj20258.top

[D04] 删除元素
来源：http://zzl.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cqc.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bfl.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hmy.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://vnv.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://udj.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://epb.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cce.gotoacloud.top

[D05] 访问与修改元素
来源：http://euy.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vyo.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zod.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sqk.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://myo.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://bnz.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://uvx.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bsj.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zsd.sjlbkw.cn

[D06] 数组长度
来源：http://fts.zycfv.cn

Py:   len(arr)
来源：http://qss.feifeiyinyue.top

PHP:  count($arr);
来源：http://jzz.gogol.net.cn

JS:   arr.length
来源：http://dhk.yj20258888.top

TS:   arr.length
来源：http://eak.dianchejie.cn

Java: list.size();
来源：http://dsz.nwbrower.top

Go:   len(arr)
来源：http://djb.xuanzx.com

Ruby: arr.length; arr.size
来源：http://njk.redwolf501.top

C#:   list.Count;
来源：http://jve.tanke756.top

[D07] 切片 / 取子数组
来源：http://vjr.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xes.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://yhv.hammf.cn

JS:   arr.slice(1, 4);
来源：http://whc.tanke756.top

TS:   arr.slice(1, 4);
来源：http://nqp.fengsongda.top

Java: list.subList(1, 4);
来源：http://hpa.jinqigufen.top

Go:   arr[1:4]
来源：http://gmq.guannengcc.top

Ruby: arr[1, 3]
来源：http://rto.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://mlp.redwolf501.top

[D08] 合并两个数组
来源：http://pwk.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://rgd.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://kjw.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hfc.sweek.top

TS:   [...a, ...b];
来源：http://cay.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wku.bjfxy.top

Go:   append(a, b...)
来源：http://vkc.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://pbb.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://trl.hnqzz.top

[D09] 排序（升序）
来源：http://omb.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://nhr.zdbjq.cn

PHP:  sort($arr);
来源：http://hnf.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xai.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yvh.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gqx.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qho.feifeiyinyue.top

Ruby: arr.sort
来源：http://ali.shanyushiyangtech.top

C#:   list.Sort();
来源：http://kbl.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ubj.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skm.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phz.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ckt.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ced.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ouc.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dmt.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jdc.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://szi.fzhhl.top

[D11] 反转数组
来源：http://meu.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://mtn.wangdashe.top

PHP:  array_reverse($arr);
来源：http://dwx.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://azm.jinqigufen.top

TS:   [...arr].reverse();
来源：http://xrf.aizwys.cn

Java: Collections.reverse(list);
来源：http://vtu.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://asb.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://msk.yj20258.top

C#:   list.Reverse();
来源：http://rvl.sjlbkw.cn

[D12] 查找元素下标
来源：http://atb.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://gkd.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uqa.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pnb.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sls.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rrg.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://ttu.uphjek.com

Ruby: arr.index(x)
来源：http://aok.xylfe.cn

C#:   list.IndexOf(x);
来源：http://nof.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://hmx.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jed.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ngd.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://ckb.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://tzt.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qwo.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbf.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://oiq.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vxv.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://flr.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fox.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fgn.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://yju.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://eip.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jfd.gaohongyu789.top

Go:   // 手写循环
来源：http://rhb.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://hln.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jkf.jinghuilouyu.cn

[D15] 去重
来源：http://nkn.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qiw.0kj1m.cn

PHP:  array_unique($arr);
来源：http://dko.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://zzn.pycfn.com

TS:   [...new Set(arr)]
来源：http://tyu.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cbo.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://hqw.aibaodan.cn

Ruby: arr.uniq
来源：http://qxr.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://qlf.guowangkeji.top

[D16] 求和与平均值
来源：http://tbl.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tpy.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eol.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dlh.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjj.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hnx.andypj.xyz

Go:   // 手写循环累加
来源：http://hhc.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nje.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://iiu.zhongyouzk.top

[D17] 最大值与最小值
来源：http://geu.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://hkr.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://ixa.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dmy.epnwcf.com

TS:   Math.max(...arr);
来源：http://sao.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://djq.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hub.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://yky.tarul.cn

C#:   list.Max();  list.Min()
来源：http://sqt.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://vbo.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ocy.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://vyy.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dpa.havefunace.top

TS:   nested.flat();
来源：http://azp.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rgg.xuanzx.com

Go:   // 手写双层循环
来源：http://csb.hammf.cn

Ruby: nested.flatten
来源：http://rcj.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uzp.dashuyun.cn

[D19] 按字段分组
来源：http://cbz.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixi.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wkn.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oyo.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://heu.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ypl.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://goo.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uwg.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rae.meibo888.top

[D20] 统计每个元素出现次数
来源：http://fdc.cashguo.top

Py:   Counter(arr)
来源：http://csy.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://dhr.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqn.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://irr.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wte.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://vnc.meibo888.top

Ruby: arr.tally
来源：http://isn.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dhd.ydzc1.top

[D21] 判断是否包含某元素
来源：http://bay.daria6918.cn

Py:   x in arr
来源：http://jsk.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://gvc.ydjk.org.cn

JS:   arr.includes(x)
来源：http://pbb.sufxvd.cn

TS:   arr.includes(x)
来源：http://mif.xuetiantiany.cn

Java: list.contains(x)
来源：http://bqk.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://uxx.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://fds.guannengcc.top

C#:   list.Contains(x)
来源：http://prw.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://bon.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://chn.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fks.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eij.zhoulong.xyz

TS:   [...arr];
来源：http://gpw.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://rat.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pcd.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://uur.wangdashe.top

C#:   new List<int>(list);
来源：http://znx.yvedp.cn

[D23] reduce 累积计算
来源：http://bbi.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://djb.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zee.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnd.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfe.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://npa.nanxuanxn.top

Go:   // 手写循环
来源：http://mvo.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qpe.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://szl.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://khc.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bnv.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ulg.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://toy.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sih.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://avv.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hgk.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vjd.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aok.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://htg.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://inq.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rni.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpb.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yam.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mhv.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://meq.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jiy.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sqv.yuxming.cn

[D26] 数组转字符串
来源：http://ody.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://dmh.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://ahq.ybcxt.top

JS:   arr.join(", ")
来源：http://xkc.ydzc1.top

TS:   arr.join(", ")
来源：http://rvx.epnwcf.com

Java: String.join(", ", list)
来源：http://jek.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://gst.fehbvm.com

Ruby: arr.join(", ")
来源：http://plp.cucudq.cn

C#:   string.Join(", ", list)
来源：http://ojr.vehdjk.com

================================================================================
来源：http://fiu.xziqi.cn

E. 字符串处理
来源：http://hjt.ivvv.top

================================================================================
来源：http://zto.xinyue.icu

[E01] 拼接字符串
来源：http://tld.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ccu.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mfh.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://syo.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://api.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://znx.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dzq.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mqv.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hkl.jqgfzy.top

[E02] 重复字符串
来源：http://igf.yangfankeji.com

Py:   "ab" * 3
来源：http://zrn.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://mxl.shuidangran.top

JS:   "ab".repeat(3)
来源：http://mno.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://jrh.yueranfly.top

Java: "ab".repeat(3)
来源：http://hgt.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://mba.jinqigfzy.top

Ruby: "ab" * 3
来源：http://wpx.aizwys.cn


<!-- 参考信息 -->