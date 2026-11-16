代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ukz.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://bxz.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://kyh.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxu.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://oac.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://uvb.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://epi.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://icv.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jnj.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://klx.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ooh.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tka.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eyr.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://whn.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jsa.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://hpj.zdqjudy.top

[C14] 泛型函数
来源：http://phm.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cku.iojbl.cn

PHP:  // 无泛型
来源：http://uyj.zycfv.cn

JS:   // 无泛型
来源：http://box.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pem.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ako.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xon.hfpthk.cn

Ruby: # 无泛型
来源：http://hbq.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vwb.andypj.xyz

[C15] 解构 / 展开参数
来源：http://wee.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mvp.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://swq.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ozg.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mep.yanxiufei.cn

Java: // 无解构
来源：http://qyw.ppjwa.cn

Go:   // 无解构
来源：http://ybe.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://nub.yuxming.cn

C#:   var (a, b) = pair;
来源：http://lpr.yvedp.cn

[C16] 函数 / 方法重载
来源：http://zne.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mdx.feifeiyinyue.top

PHP:  // 无重载
来源：http://axq.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ooi.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://tgb.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://vhx.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://cbp.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://hiy.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oks.jqgfzy.top

================================================================================
来源：http://zyj.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://fpq.dashuyun.cn

================================================================================
来源：http://kpv.c1oappe.top

[D01] 创建数组 / 列表
来源：http://hjd.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vvt.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fjn.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lgs.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qkw.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lgc.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://avw.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://kkb.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ora.jiagoushi.top

[D02] 追加元素到末尾
来源：http://yse.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qkq.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sce.yj20258.top

JS:   arr.push(4);
来源：http://hnq.haohaochexian.top

TS:   arr.push(4);
来源：http://atq.jinqigfzy.top

Java: list.add(4);
来源：http://irw.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://vhv.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://dqs.jlsjyb.cn

C#:   list.Add(4);
来源：http://czb.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://hrr.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://waa.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlg.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iqd.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://hbq.jinqigufen.top

Java: list.add(0, 0);
来源：http://tev.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://gij.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gnb.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://ina.ppjwa.cn

[D04] 删除元素
来源：http://dot.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ryu.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uof.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xeo.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://edw.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wpd.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ahb.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qel.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fjw.vqdsnc.cn

[D05] 访问与修改元素
来源：http://jwk.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://une.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pxj.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gvi.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://aat.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://vjn.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://huy.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gql.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rrt.yj202588.top

[D06] 数组长度
来源：http://djr.ivvv.top

Py:   len(arr)
来源：http://uih.redwolf501.top

PHP:  count($arr);
来源：http://gup.jlsjyb.cn

JS:   arr.length
来源：http://oua.jinyuanbaomall.cn

TS:   arr.length
来源：http://inl.jqgfzy.top

Java: list.size();
来源：http://vsr.tianlin.xyz

Go:   len(arr)
来源：http://sap.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://phn.xuanzx.com

C#:   list.Count;
来源：http://hyr.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://zpz.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://alp.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nni.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://afh.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://crg.nwbrower.top

Java: list.subList(1, 4);
来源：http://bqi.fengsongda.top

Go:   arr[1:4]
来源：http://fsr.hesvh.cn

Ruby: arr[1, 3]
来源：http://fxy.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://dtp.guannengcc.top

[D08] 合并两个数组
来源：http://lrt.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://niv.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://dzh.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ooe.ehwqpu.com

TS:   [...a, ...b];
来源：http://wke.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://awh.cheryme.top

Go:   append(a, b...)
来源：http://nie.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://xer.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://avy.sufxvd.cn

[D09] 排序（升序）
来源：http://quk.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://gyt.jianghu66.top

PHP:  sort($arr);
来源：http://zwc.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lym.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nyr.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dvj.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bta.kuanghao11.cn

Ruby: arr.sort
来源：http://rmu.hfpthk.cn

C#:   list.Sort();
来源：http://czn.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bln.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lxq.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qbv.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvl.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rxc.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jda.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zdt.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mhg.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bko.cqqwz.cn

[D11] 反转数组
来源：http://sed.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://wml.cashguo.top

PHP:  array_reverse($arr);
来源：http://ior.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kjz.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://ahq.haohaochexian.top

Java: Collections.reverse(list);
来源：http://nph.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://lzx.gaohongyu789.top

Ruby: arr.reverse
来源：http://duk.sjlbkw.cn

C#:   list.Reverse();
来源：http://hof.hammf.cn

[D12] 查找元素下标
来源：http://uta.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://zpj.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ypz.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jss.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chu.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kra.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://qwi.cheryme.top

Ruby: arr.index(x)
来源：http://fio.yvedp.cn

C#:   list.IndexOf(x);
来源：http://gbi.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://vop.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oeb.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sgx.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://dga.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://gbt.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zqf.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://woq.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://nhv.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://glc.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://vll.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jjj.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jul.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://kxi.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://ytl.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kir.dianchejie.cn

Go:   // 手写循环
来源：http://cvq.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://sqb.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gzp.jinqigufen.top

[D15] 去重
来源：http://shv.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cmn.svipenyu.cn

PHP:  array_unique($arr);
来源：http://rmj.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://tjw.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://fax.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iac.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://ksb.gogol.net.cn

Ruby: arr.uniq
来源：http://ogg.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://cbx.jinqigufen.top

[D16] 求和与平均值
来源：http://gya.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hgo.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cds.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bnd.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdj.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ryh.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://pjv.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kug.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://roj.xylfe.cn

[D17] 最大值与最小值
来源：http://vay.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://ijn.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://cbr.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://efp.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://piu.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bmz.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mrw.pycfn.com

Ruby: arr.max;  arr.min
来源：http://zph.cashguo.top

C#:   list.Max();  list.Min()
来源：http://hvu.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://ivc.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hqp.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://vtu.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qhs.ivvv.top

TS:   nested.flat();
来源：http://cwf.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ulg.fehbvm.com

Go:   // 手写双层循环
来源：http://usw.gotoacloud.top

Ruby: nested.flatten
来源：http://gcd.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://ktt.xuanzx.com

[D19] 按字段分组
来源：http://ucv.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ifr.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nyq.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ztx.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://izf.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ovj.cashguo.top

Go:   // 手写 map[string][]T
来源：http://emq.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://spt.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ypi.tarul.cn

[D20] 统计每个元素出现次数
来源：http://ssz.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://pzv.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://mka.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ucx.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fmr.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iky.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://euh.guannengcc.top

Ruby: arr.tally
来源：http://xmi.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rdk.bjfxy.top

[D21] 判断是否包含某元素
来源：http://tgg.hnxiangtu.top

Py:   x in arr
来源：http://rpp.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://lbz.dashuyun.cn

JS:   arr.includes(x)
来源：http://xak.daria6918.cn

TS:   arr.includes(x)
来源：http://xyi.shzxlz.cn

Java: list.contains(x)
来源：http://oba.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://sjj.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://hiu.andypj.xyz

C#:   list.Contains(x)
来源：http://vnj.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://qyv.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axn.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://drq.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://owl.xziqi.cn

TS:   [...arr];
来源：http://mxq.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://sxe.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://lqt.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://nqw.meibo888.top

C#:   new List<int>(list);
来源：http://wge.hesvh.cn

[D23] reduce 累积计算
来源：http://hjy.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dym.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mre.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wzd.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ayb.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yom.jianghu66.top

Go:   // 手写循环
来源：http://obb.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cjg.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iva.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://jzu.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lqv.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pot.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kqq.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zhx.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rjx.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ddp.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://giw.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kyf.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://you.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://url.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://unw.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hoc.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hkk.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://usv.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vvk.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rig.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tzf.uphjek.com

[D26] 数组转字符串
来源：http://miv.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://tct.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://sbu.jyoumei.cn

JS:   arr.join(", ")
来源：http://ive.gogol.net.cn

TS:   arr.join(", ")
来源：http://pve.jqgfzy.top

Java: String.join(", ", list)
来源：http://ith.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://dmy.guowangkeji.top

Ruby: arr.join(", ")
来源：http://cbk.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://wbs.guowangkeji.top

================================================================================
来源：http://axj.nanxinkj.top

E. 字符串处理
来源：http://yxx.yj20258.top

================================================================================
来源：http://lmr.kuanghao11.cn

[E01] 拼接字符串
来源：http://dkc.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yzh.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tey.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kmm.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://del.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fxo.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zik.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yrs.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tmg.jyoumei.cn

[E02] 重复字符串
来源：http://iye.xziqi.cn

Py:   "ab" * 3
来源：http://cul.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://pun.sxryk.cn

JS:   "ab".repeat(3)
来源：http://mah.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://lmb.sysykeji.top

Java: "ab".repeat(3)
来源：http://kwj.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://fyj.sjlbkw.cn

Ruby: "ab" * 3
来源：http://uzr.ydjk.org.cn


<!-- 参考信息 -->