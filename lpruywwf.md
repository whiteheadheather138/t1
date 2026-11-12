代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://iuy.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://qjq.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yti.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://zpu.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cpz.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://joj.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vpn.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hhi.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kpd.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://nrz.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rev.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://gyd.0kj1m.cn

[C14] 泛型函数
来源：http://zgv.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hwl.yj20258.top

PHP:  // 无泛型
来源：http://jhi.jqgufenzy.top

JS:   // 无泛型
来源：http://fgl.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tvg.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uia.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eaw.hammf.cn

Ruby: # 无泛型
来源：http://ygs.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uii.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://ogr.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rbx.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://jzf.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qzg.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pdg.cucudq.cn

Java: // 无解构
来源：http://sjz.guowangkeji.top

Go:   // 无解构
来源：http://fbs.jlsjyb.cn

Ruby: a, b = pair
来源：http://cen.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://iwe.316326.xyz

[C16] 函数 / 方法重载
来源：http://qba.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sol.cdnleiting.top

PHP:  // 无重载
来源：http://tsh.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mkj.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://ubx.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://daf.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://hfn.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://mwc.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wku.yonumen.top

================================================================================
来源：http://usf.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://szy.xziqi.cn

================================================================================
来源：http://azo.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://xhy.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwc.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dav.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://owa.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pyc.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ksa.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://ssd.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://jdy.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ixc.ivvv.top

[D02] 追加元素到末尾
来源：http://tfm.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hzz.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bqf.yfazqb.com

JS:   arr.push(4);
来源：http://heg.chenzaomai.com

TS:   arr.push(4);
来源：http://thv.yj202588.top

Java: list.add(4);
来源：http://ecb.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://rpj.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://opc.daria6918.cn

C#:   list.Add(4);
来源：http://tlz.bbcook.cn

[D03] 在指定位置插入元素
来源：http://pqz.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://qks.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gqd.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xzw.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://ihw.gotoacloud.top

Java: list.add(0, 0);
来源：http://han.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://irh.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sey.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://bor.birdmap.top

[D04] 删除元素
来源：http://hqg.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zpj.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmi.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://geq.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://wwp.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gtg.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://csg.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mpm.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gwh.vehdjk.com

[D05] 访问与修改元素
来源：http://nsr.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cem.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qlb.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gth.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://lll.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://vqt.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://gws.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mxh.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fjo.fanxiaobao.xyz

[D06] 数组长度
来源：http://jus.jinqigfzy.top

Py:   len(arr)
来源：http://dzd.jinqigufen.top

PHP:  count($arr);
来源：http://xhi.ehwqpu.com

JS:   arr.length
来源：http://jsv.316326.xyz

TS:   arr.length
来源：http://mau.xziqi.cn

Java: list.size();
来源：http://wtf.yueranfly.top

Go:   len(arr)
来源：http://ndh.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://yzz.redwolf501.top

C#:   list.Count;
来源：http://vlk.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://wor.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywp.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xws.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://zsi.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://ikg.yj20258.top

Java: list.subList(1, 4);
来源：http://wvv.yueranfly.top

Go:   arr[1:4]
来源：http://jed.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://vua.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://fqx.zycfv.cn

[D08] 合并两个数组
来源：http://bxd.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://nru.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://hyr.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zoy.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://vti.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smj.ivvv.top

Go:   append(a, b...)
来源：http://ziq.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://cbx.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://mku.kuanghao11.cn

[D09] 排序（升序）
来源：http://fyt.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://nps.yj20258.top

PHP:  sort($arr);
来源：http://yyr.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mgx.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fub.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tcw.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://byq.ehwqpu.com

Ruby: arr.sort
来源：http://czf.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://urz.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wzc.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jvn.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nue.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mhb.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://opi.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtk.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ezl.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qpe.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nto.vehdjk.com

[D11] 反转数组
来源：http://ram.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://fpg.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://adb.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vpl.sufxvd.cn

TS:   [...arr].reverse();
来源：http://bzs.yangfankeji.com

Java: Collections.reverse(list);
来源：http://hln.tarul.cn

Go:   slices.Reverse(arr)
来源：http://evg.yuxming.cn

Ruby: arr.reverse
来源：http://sqb.yongpay.top

C#:   list.Reverse();
来源：http://mfd.gzhubu.top

[D12] 查找元素下标
来源：http://ozs.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://hcs.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xoe.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ibt.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ggf.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ktq.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://nhy.jqgufenzy.top

Ruby: arr.index(x)
来源：http://adr.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://mtm.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://uwy.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rag.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cpf.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://yfr.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://pjb.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kci.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://umd.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://mst.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://afi.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://pxa.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://muf.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://twx.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://jml.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://tnr.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ine.jqgfzy.top

Go:   // 手写循环
来源：http://jso.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aac.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ppd.fanxiaobao.xyz

[D15] 去重
来源：http://dxv.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://usd.316326.xyz

PHP:  array_unique($arr);
来源：http://oui.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://kjp.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://pta.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kfk.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fcx.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://ysw.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://mql.9152youxi.cn

[D16] 求和与平均值
来源：http://ixg.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rxy.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://twz.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yfc.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://unw.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tku.jiagoushi.top

Go:   // 手写循环累加
来源：http://grc.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fba.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://ayg.xylfe.cn

[D17] 最大值与最小值
来源：http://ros.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://ukh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://lzw.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wnv.ehwqpu.com

TS:   Math.max(...arr);
来源：http://mts.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ahq.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nnv.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://tum.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://tzi.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://slb.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rus.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://yvb.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lub.mhx1999.top

TS:   nested.flat();
来源：http://kes.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tid.cdnleiting.top

Go:   // 手写双层循环
来源：http://pif.dianchejie.cn

Ruby: nested.flatten
来源：http://psu.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sfp.ppjwa.cn

[D19] 按字段分组
来源：http://rag.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dgk.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cpl.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dsk.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tka.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ipf.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://hfd.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rfo.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cln.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://zan.jqgufenzy.top

Py:   Counter(arr)
来源：http://hll.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://pxn.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mxh.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgf.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hmg.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://wox.iojbl.cn

Ruby: arr.tally
来源：http://xfd.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wcr.yfazqb.com

[D21] 判断是否包含某元素
来源：http://hex.gaohongyu789.top

Py:   x in arr
来源：http://lgv.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://lmt.haohaochexian.top

JS:   arr.includes(x)
来源：http://hmn.cashguo.top

TS:   arr.includes(x)
来源：http://xsl.316326.xyz

Java: list.contains(x)
来源：http://wkd.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://clc.nwbrower.top

Ruby: arr.include?(x)
来源：http://nay.jyoumei.cn

C#:   list.Contains(x)
来源：http://djb.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://zxi.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kue.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lhy.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vwu.52xcode.cn

TS:   [...arr];
来源：http://tpn.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://oay.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ytt.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://whl.iojbl.cn

C#:   new List<int>(list);
来源：http://xhh.bbcook.cn

[D23] reduce 累积计算
来源：http://fqa.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pyi.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lzs.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blk.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fge.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hqp.hysaishi.cn

Go:   // 手写循环
来源：http://dyr.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zgi.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lxt.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://csu.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xka.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hfr.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aha.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cjh.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mrp.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqz.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ctk.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kow.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://hcc.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tot.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hxs.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://htr.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fer.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whp.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rvg.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hry.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nuu.pengpengdd.cyou

[D26] 数组转字符串
来源：http://naq.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://dcs.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://tjv.sufxvd.cn

JS:   arr.join(", ")
来源：http://dfo.aibaodan.cn

TS:   arr.join(", ")
来源：http://naq.dashuyun.cn

Java: String.join(", ", list)
来源：http://ebj.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://jsz.gogol.net.cn

Ruby: arr.join(", ")
来源：http://bvn.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://cxn.gaohongyu789.top

================================================================================
来源：http://iou.hammf.cn

E. 字符串处理
来源：http://dfq.wangdashe.top

================================================================================
来源：http://ikc.yfazqb.com

[E01] 拼接字符串
来源：http://sxw.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xde.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://esf.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xwu.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://epv.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zlh.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ina.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eci.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ykh.tanke756.top

[E02] 重复字符串
来源：http://wma.yanxiufei.cn

Py:   "ab" * 3
来源：http://drd.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://jod.bjfxy.top

JS:   "ab".repeat(3)
来源：http://zdf.vehdjk.com

TS:   "ab".repeat(3)
来源：http://ogr.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://omj.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://lom.ydjk.org.cn

Ruby: "ab" * 3
来源：http://kmj.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dpk.chenzaomai.com

[E03] 截取子串
来源：http://xsy.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyt.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dux.gaohongyu789.top


<!-- 参考信息 -->