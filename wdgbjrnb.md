代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eym.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iok.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jjq.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbq.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zsh.guowangkeji.top

Go:   func add(a, b int) int
来源：http://qjz.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pgu.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://upc.guannengcc.top

[C14] 泛型函数
来源：http://fbj.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbp.fengsongda.top

PHP:  // 无泛型
来源：http://vex.316326.xyz

JS:   // 无泛型
来源：http://rxt.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ykc.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bld.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://szd.aibaodan.cn

Ruby: # 无泛型
来源：http://iaf.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncu.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://bco.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ogs.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://vxe.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lpt.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uqd.xylfe.cn

Java: // 无解构
来源：http://ejh.tarul.cn

Go:   // 无解构
来源：http://tpi.bbcook.cn

Ruby: a, b = pair
来源：http://qkh.ydzc1.top

C#:   var (a, b) = pair;
来源：http://nmc.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://klq.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wiz.birdmap.top

PHP:  // 无重载
来源：http://lot.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qni.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zdn.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://usa.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://hrk.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://ofz.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fah.yangfankeji.com

================================================================================
来源：http://gzr.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://pqw.shzxlz.cn

================================================================================
来源：http://jrw.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://lwc.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ubu.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://och.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fne.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://asd.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hhw.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://trd.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://nmw.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uio.xinyue.icu

[D02] 追加元素到末尾
来源：http://cfz.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zbb.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dfu.shzxlz.cn

JS:   arr.push(4);
来源：http://emg.yongpay.top

TS:   arr.push(4);
来源：http://bkd.shanyushiyangkeji.top

Java: list.add(4);
来源：http://zjq.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://wfh.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://mor.fehbvm.com

C#:   list.Add(4);
来源：http://ccc.sweek.top

[D03] 在指定位置插入元素
来源：http://hdh.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://xms.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bwy.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gsm.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://udv.smart0.xyz

Java: list.add(0, 0);
来源：http://mdz.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://uix.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jah.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://ext.jianghu66.top

[D04] 删除元素
来源：http://qog.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zhl.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wuo.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wdl.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://pfb.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mug.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nui.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dhd.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://itx.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://gfe.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ofo.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://emh.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xxk.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://fqe.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://vbf.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://usa.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tsi.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yhv.yuxming.cn

[D06] 数组长度
来源：http://gud.cqqwz.cn

Py:   len(arr)
来源：http://rsi.tarul.cn

PHP:  count($arr);
来源：http://vbc.hfpthk.cn

JS:   arr.length
来源：http://mvc.shanyushiyangtech.top

TS:   arr.length
来源：http://vqw.ybcxt.top

Java: list.size();
来源：http://itj.jiagoushi.top

Go:   len(arr)
来源：http://vzx.hammf.cn

Ruby: arr.length; arr.size
来源：http://des.iojbl.cn

C#:   list.Count;
来源：http://dmd.xuanzx.com

[D07] 切片 / 取子数组
来源：http://afs.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dim.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bno.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://fty.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://rwc.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://naz.jyoumei.cn

Go:   arr[1:4]
来源：http://slv.guowangkeji.top

Ruby: arr[1, 3]
来源：http://wqb.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://hdy.havefunace.top

[D08] 合并两个数组
来源：http://cei.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://ggb.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://gri.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oai.jqgufenzy.top

TS:   [...a, ...b];
来源：http://dbs.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vey.nwbrower.top

Go:   append(a, b...)
来源：http://crb.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://ijl.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://gpm.sweek.top

[D09] 排序（升序）
来源：http://ioa.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://pmw.fengsongda.top

PHP:  sort($arr);
来源：http://wcb.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://byx.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://now.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ycm.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qjw.ctjpmb.com

Ruby: arr.sort
来源：http://lry.jianghu66.top

C#:   list.Sort();
来源：http://ydn.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zsm.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bfa.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://usm.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfs.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://spx.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ant.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mmd.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nmu.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jbk.dashuyun.cn

[D11] 反转数组
来源：http://odq.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://zpq.zycfv.cn

PHP:  array_reverse($arr);
来源：http://zyi.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dxo.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://omz.ehwqpu.com

Java: Collections.reverse(list);
来源：http://zce.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://zym.daria6918.cn

Ruby: arr.reverse
来源：http://zzy.zhijiandao.cn

C#:   list.Reverse();
来源：http://yqr.9152youxi.cn

[D12] 查找元素下标
来源：http://tpr.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://esb.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pjn.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brh.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bbx.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://usy.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://lpq.xinyue.icu

Ruby: arr.index(x)
来源：http://cut.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://smk.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://wjl.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://glr.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bne.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://xxk.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://hsx.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xbm.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iqu.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://lxn.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ido.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://izz.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nwj.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bpv.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://cbw.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://zjh.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://utv.9152youxi.cn

Go:   // 手写循环
来源：http://flz.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://yku.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dsz.aizwys.cn

[D15] 去重
来源：http://rrk.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pdb.shzxlz.cn

PHP:  array_unique($arr);
来源：http://xhb.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://imx.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://kpv.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fkn.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://iqh.shzxlz.cn

Ruby: arr.uniq
来源：http://lnu.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://xde.52xcode.cn

[D16] 求和与平均值
来源：http://alo.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cyc.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wpf.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jtj.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vhe.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dmc.yangfankeji.com

Go:   // 手写循环累加
来源：http://jsx.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emw.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://psk.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://zet.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://ejj.sweek.top

PHP:  max($arr);  min($arr);
来源：http://alm.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://orc.wangdashe.top

TS:   Math.max(...arr);
来源：http://mqm.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tcv.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lqw.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://ztq.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://lvs.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://xyg.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kug.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://pyo.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://awd.nanxuanxn.top

TS:   nested.flat();
来源：http://zcy.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fjs.ehwqpu.com

Go:   // 手写双层循环
来源：http://abu.chenzaomai.com

Ruby: nested.flatten
来源：http://dyy.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jur.cqqwz.cn

[D19] 按字段分组
来源：http://qsm.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mrj.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fia.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xbh.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lhf.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hzw.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://loz.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xyz.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vnv.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://qyb.mhx1999.top

Py:   Counter(arr)
来源：http://csp.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://hhf.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jsu.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skt.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lan.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://nat.cucudq.cn

Ruby: arr.tally
来源：http://nng.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ftg.redwolf501.top

[D21] 判断是否包含某元素
来源：http://xbr.hfpthk.cn

Py:   x in arr
来源：http://jrs.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://gva.dianchejie.cn

JS:   arr.includes(x)
来源：http://itp.yanxiufei.cn

TS:   arr.includes(x)
来源：http://ktp.chenzaomai.com

Java: list.contains(x)
来源：http://hdl.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://goe.ctjpmb.com

Ruby: arr.include?(x)
来源：http://fgg.yanxiufei.cn

C#:   list.Contains(x)
来源：http://xvv.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://eqk.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oha.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://umv.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fpr.tianlin.xyz

TS:   [...arr];
来源：http://xbw.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://bnz.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lry.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://wzh.gaohongyu789.top

C#:   new List<int>(list);
来源：http://jhk.pycfn.com

[D23] reduce 累积计算
来源：http://zqk.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rwg.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bbs.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yhe.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rug.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ism.fengsongda.top

Go:   // 手写循环
来源：http://zhh.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhu.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dmh.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://che.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pkp.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://djm.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zyv.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wff.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vof.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ioa.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aqv.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pez.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://fud.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lna.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hfl.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lrn.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://csz.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ely.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hoc.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kzo.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://for.sjlbkw.cn

[D26] 数组转字符串
来源：http://oyu.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://lgz.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://ogw.hesvh.cn

JS:   arr.join(", ")
来源：http://zad.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://xst.dianchejie.cn

Java: String.join(", ", list)
来源：http://rgr.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://vcv.jyoumei.cn

Ruby: arr.join(", ")
来源：http://bwh.yj202588.top

C#:   string.Join(", ", list)
来源：http://rax.aizwys.cn

================================================================================
来源：http://noo.gotoacloud.top

E. 字符串处理
来源：http://mxv.mhx1999.top

================================================================================
来源：http://mmi.zdbjq.cn

[E01] 拼接字符串
来源：http://mhu.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zde.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zoq.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ary.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmg.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vyn.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nvo.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fpe.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zwx.yvedp.cn

[E02] 重复字符串
来源：http://noi.hnxiangtu.top

Py:   "ab" * 3
来源：http://ddm.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://tln.sysykeji.top

JS:   "ab".repeat(3)
来源：http://njz.zycfv.cn

TS:   "ab".repeat(3)
来源：http://gvh.zhengqikj.top

Java: "ab".repeat(3)
来源：http://ryq.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://vsp.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://ugl.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xxo.hnxiangtu.top

[E03] 截取子串
来源：http://oft.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bap.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oda.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zka.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://ekg.hammf.cn

Java: s.substring(1, 4)
来源：http://ypp.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://itx.quarkkingdee.top


<!-- 参考信息 -->