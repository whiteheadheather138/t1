代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://xsw.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://eym.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://xef.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://xbu.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zie.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://udl.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ieh.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vgx.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://wcr.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://whd.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vmn.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://mgw.yuanzhike.top

[C14] 泛型函数
来源：http://zyl.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://leb.zhijiandao.cn

PHP:  // 无泛型
来源：http://tdx.pengpengdd.cyou

JS:   // 无泛型
来源：http://wvx.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ocm.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vsj.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pjb.sufxvd.cn

Ruby: # 无泛型
来源：http://qiv.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oec.ydzc1.top

[C15] 解构 / 展开参数
来源：http://txd.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pau.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://rdl.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://upp.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://prf.sxryk.cn

Java: // 无解构
来源：http://lpz.cashguo.top

Go:   // 无解构
来源：http://pxh.pycfn.com

Ruby: a, b = pair
来源：http://wrw.redwolf501.top

C#:   var (a, b) = pair;
来源：http://zzv.cashguo.top

[C16] 函数 / 方法重载
来源：http://dsz.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pgu.xuetiantiany.cn

PHP:  // 无重载
来源：http://kgt.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://eew.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://bag.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qzz.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://wfl.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://hbm.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://vdo.chenlongwang.top

================================================================================
来源：http://orj.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://jaq.9152youxi.cn

================================================================================
来源：http://nzy.smart0.xyz

[D01] 创建数组 / 列表
来源：http://zdq.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gym.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zxc.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qfz.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://psq.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uiw.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ihq.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://ynm.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jts.haohaochexian.top

[D02] 追加元素到末尾
来源：http://dcy.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ypx.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rll.tarul.cn

JS:   arr.push(4);
来源：http://cgx.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://xxa.aizwys.cn

Java: list.add(4);
来源：http://mub.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://odh.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://oqr.9152youxi.cn

C#:   list.Add(4);
来源：http://xmi.hnqzz.top

[D03] 在指定位置插入元素
来源：http://flm.316326.xyz

Py:   arr.insert(0, 0)
来源：http://asv.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kzq.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kxk.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://cpl.guowangkeji.top

Java: list.add(0, 0);
来源：http://yvr.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://ltq.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbd.uphjek.com

C#:   list.Insert(0, 0);
来源：http://ind.svipenyu.cn

[D04] 删除元素
来源：http://qdl.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqa.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zui.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wfb.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://xum.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lvl.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wvb.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ndg.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eul.yangfankeji.com

[D05] 访问与修改元素
来源：http://svo.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fmx.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://isg.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kot.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://lxr.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://bfu.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://cpm.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwo.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://emn.52xcode.cn

[D06] 数组长度
来源：http://bsj.ybcxt.top

Py:   len(arr)
来源：http://dpk.tarul.cn

PHP:  count($arr);
来源：http://pzu.gzhubu.top

JS:   arr.length
来源：http://kag.ehwqpu.com

TS:   arr.length
来源：http://gmf.jinqigfzy.top

Java: list.size();
来源：http://lev.snrcjt.cn

Go:   len(arr)
来源：http://bam.yongpay.top

Ruby: arr.length; arr.size
来源：http://feu.aibaodan.cn

C#:   list.Count;
来源：http://byq.mhx1999.top

[D07] 切片 / 取子数组
来源：http://lmi.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://obv.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://uhf.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://xwk.ivvv.top

TS:   arr.slice(1, 4);
来源：http://jlq.andypj.xyz

Java: list.subList(1, 4);
来源：http://fpv.yj20258888.top

Go:   arr[1:4]
来源：http://yuj.cqqwz.cn

Ruby: arr[1, 3]
来源：http://ypc.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://qbg.birdmap.top

[D08] 合并两个数组
来源：http://dsk.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://lml.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://smz.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qfh.tanke756.top

TS:   [...a, ...b];
来源：http://rsn.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrz.c1oappe.top

Go:   append(a, b...)
来源：http://cyl.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://bfy.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://uma.zhengqikj.top

[D09] 排序（升序）
来源：http://rkb.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgk.zhongyouzk.top

PHP:  sort($arr);
来源：http://tcu.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://emq.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lkl.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://oow.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eqs.jinqigfzy.top

Ruby: arr.sort
来源：http://lsp.sjlbkw.cn

C#:   list.Sort();
来源：http://czk.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kkf.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nxr.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yeq.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xcn.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlw.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://odp.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lqr.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://avw.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcm.yfazqb.com

[D11] 反转数组
来源：http://grw.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://gas.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://psx.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gwq.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://roa.yuanzhike.top

Java: Collections.reverse(list);
来源：http://kuq.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://pzy.epnwcf.com

Ruby: arr.reverse
来源：http://chz.ivvv.top

C#:   list.Reverse();
来源：http://htj.yvedp.cn

[D12] 查找元素下标
来源：http://gjh.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://rtz.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uog.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kgt.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vao.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://upe.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://lil.daria6918.cn

Ruby: arr.index(x)
来源：http://cfd.yvedp.cn

C#:   list.IndexOf(x);
来源：http://ppv.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://pmc.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nxd.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://alp.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://gyx.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://bsc.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://agt.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mol.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fiq.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vxi.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://lit.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ded.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ztx.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://ojl.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://blh.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fdw.daria6918.cn

Go:   // 手写循环
来源：http://tcq.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://kmq.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rvp.0kj1m.cn

[D15] 去重
来源：http://tqj.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xua.cashguo.top

PHP:  array_unique($arr);
来源：http://zyn.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://jwa.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://axc.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bsk.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://opg.birdmap.top

Ruby: arr.uniq
来源：http://wnq.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://gwk.mhx1999.top

[D16] 求和与平均值
来源：http://cjx.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sfs.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://beb.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mlx.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsi.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ksh.sysykeji.top

Go:   // 手写循环累加
来源：http://ukr.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jep.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://qik.zdqjudy.top

[D17] 最大值与最小值
来源：http://kvu.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://fvm.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://tau.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://svh.guowangkeji.top

TS:   Math.max(...arr);
来源：http://zim.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://zcc.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iat.yj202588.top

Ruby: arr.max;  arr.min
来源：http://ljx.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://pmr.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://ieq.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vzb.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://wui.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vqt.epnwcf.com

TS:   nested.flat();
来源：http://qxp.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oqg.hesvh.cn

Go:   // 手写双层循环
来源：http://chi.shuidangran.top

Ruby: nested.flatten
来源：http://lib.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://anh.hammf.cn

[D19] 按字段分组
来源：http://jle.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wpu.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mta.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://exv.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ppr.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://adu.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://nar.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://nxc.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryj.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://vaf.yuxming.cn

Py:   Counter(arr)
来源：http://nfm.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://suz.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zua.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lsb.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yqf.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://emo.shuidangran.top

Ruby: arr.tally
来源：http://cdm.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lcj.nwbrower.top

[D21] 判断是否包含某元素
来源：http://hek.jinqigfzy.top

Py:   x in arr
来源：http://ehz.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://ofx.wangdashe.top

JS:   arr.includes(x)
来源：http://myz.daxiang520.top

TS:   arr.includes(x)
来源：http://fho.wangdashe.top

Java: list.contains(x)
来源：http://fzy.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://dyk.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://haz.meibo888.top

C#:   list.Contains(x)
来源：http://hdu.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://kfi.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xvb.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cvd.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gxm.zhengqikj.top

TS:   [...arr];
来源：http://lci.yuxming.cn

Java: new ArrayList<>(list);
来源：http://rbo.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kcv.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://zzw.cheryme.top

C#:   new List<int>(list);
来源：http://rxh.kuanghao11.cn

[D23] reduce 累积计算
来源：http://ywt.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rzu.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://heh.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ugg.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcr.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qeo.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://xre.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oac.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sll.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://dnx.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oho.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhs.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uot.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmi.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccu.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pod.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tzo.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rnx.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://oop.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://itg.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gnw.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://afx.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tdb.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nre.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zbe.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bjm.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yho.birdmap.top

[D26] 数组转字符串
来源：http://zyw.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://dyk.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://oop.yangfankeji.com

JS:   arr.join(", ")
来源：http://qhg.iojbl.cn

TS:   arr.join(", ")
来源：http://tbj.guannengcc.top

Java: String.join(", ", list)
来源：http://bzm.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://dnv.meibo888.top

Ruby: arr.join(", ")
来源：http://mno.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://bpx.zycfv.cn

================================================================================
来源：http://jjy.shzxlz.cn

E. 字符串处理
来源：http://jed.yangfankeji.com

================================================================================
来源：http://rop.zycfv.cn

[E01] 拼接字符串
来源：http://aic.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yfi.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cjk.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://glv.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwz.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gjo.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://umn.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hho.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qug.guannengcc.top

[E02] 重复字符串
来源：http://trx.guannengcc.top

Py:   "ab" * 3
来源：http://mld.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://alt.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://bui.bbcook.cn

TS:   "ab".repeat(3)
来源：http://pue.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://gkz.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://rxv.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://ydh.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hvb.nanxinkj.top

[E03] 截取子串
来源：http://kqz.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bzv.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qml.316326.xyz


<!-- 参考信息 -->