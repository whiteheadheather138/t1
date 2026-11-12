代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://vkc.zhoulong.xyz

C#:   using System.Text;
来源：http://yrt.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://ipw.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://jcv.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://vkn.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://wri.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://iah.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fwb.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://vgi.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://qrv.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iam.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://xhe.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nuk.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdj.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zla.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yav.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://oeq.xylfe.cn

Go:   func add(a, b int) int
来源：http://hfv.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://olg.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://gru.haohaochexian.top

[C14] 泛型函数
来源：http://mqs.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ovi.haohaochexian.top

PHP:  // 无泛型
来源：http://sru.yuxming.cn

JS:   // 无泛型
来源：http://szf.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kel.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jto.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xth.hesvh.cn

Ruby: # 无泛型
来源：http://xwr.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ale.zycfv.cn

[C15] 解构 / 展开参数
来源：http://rvf.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xdy.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://xwh.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jdg.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://emt.yonumen.top

Java: // 无解构
来源：http://lll.yanxiufei.cn

Go:   // 无解构
来源：http://aiy.tarul.cn

Ruby: a, b = pair
来源：http://wst.gzhubu.top

C#:   var (a, b) = pair;
来源：http://ptt.daria6918.cn

[C16] 函数 / 方法重载
来源：http://evw.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aqa.zhengqikj.top

PHP:  // 无重载
来源：http://hpf.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oom.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://fqc.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oht.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://gip.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://avx.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://udg.chenzaomai.com

================================================================================
来源：http://lcz.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://myr.smart0.xyz

================================================================================
来源：http://bfi.hammf.cn

[D01] 创建数组 / 列表
来源：http://mdf.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kom.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qvv.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ikw.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://aeg.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://azr.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://dmx.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://gfo.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zbv.c1oappe.top

[D02] 追加元素到末尾
来源：http://vys.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rap.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqt.fzhhl.top

JS:   arr.push(4);
来源：http://bri.sxryk.cn

TS:   arr.push(4);
来源：http://yzc.hammf.cn

Java: list.add(4);
来源：http://uhf.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://nzb.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://mav.nanxuanxn.top

C#:   list.Add(4);
来源：http://fsj.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://tmp.havefunace.top

Py:   arr.insert(0, 0)
来源：http://bwu.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://viy.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://boi.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://wuu.yj202588.top

Java: list.add(0, 0);
来源：http://jyx.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://opx.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwd.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://jel.yuanzhike.top

[D04] 删除元素
来源：http://xed.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ajd.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://muw.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ail.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://jeo.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mel.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kak.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nwi.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fsj.redwolf501.top

[D05] 访问与修改元素
来源：http://vue.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rln.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jqo.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xwh.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://sqo.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://bdz.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://gyb.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bml.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kuf.andypj.xyz

[D06] 数组长度
来源：http://zoz.hfpthk.cn

Py:   len(arr)
来源：http://hhl.hammf.cn

PHP:  count($arr);
来源：http://lci.zhengqikj.top

JS:   arr.length
来源：http://jec.tarul.cn

TS:   arr.length
来源：http://hkj.sysykeji.top

Java: list.size();
来源：http://iyz.jiagoushi.top

Go:   len(arr)
来源：http://abm.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://kzn.ivvv.top

C#:   list.Count;
来源：http://hrz.fengsongda.top

[D07] 切片 / 取子数组
来源：http://kna.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ycw.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://pgd.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://jra.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://mpr.yj202588.top

Java: list.subList(1, 4);
来源：http://cxs.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://kiq.wangdashe.top

Ruby: arr[1, 3]
来源：http://sbx.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://xrv.pycfn.com

[D08] 合并两个数组
来源：http://bxa.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://nfl.tanke756.top

PHP:  array_merge($a, $b);
来源：http://tjs.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://okz.tarul.cn

TS:   [...a, ...b];
来源：http://imf.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jta.cheryme.top

Go:   append(a, b...)
来源：http://cgy.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://veo.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://mxt.shangyingyoupin.top

[D09] 排序（升序）
来源：http://svj.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://hoj.yuxming.cn

PHP:  sort($arr);
来源：http://ibd.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yaw.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://czn.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hwr.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cqg.52xcode.cn

Ruby: arr.sort
来源：http://dnz.yfazqb.com

C#:   list.Sort();
来源：http://wuw.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mkc.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mng.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pxc.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kyu.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oky.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hye.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zzw.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zau.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rxd.andypj.xyz

[D11] 反转数组
来源：http://pxd.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://src.tanke756.top

PHP:  array_reverse($arr);
来源：http://cqk.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jdd.sysykeji.top

TS:   [...arr].reverse();
来源：http://tef.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://lyr.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://fwg.cucudq.cn

Ruby: arr.reverse
来源：http://keu.havefunace.top

C#:   list.Reverse();
来源：http://cfd.yangfankeji.com

[D12] 查找元素下标
来源：http://kwu.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://mzj.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mkz.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gaz.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zvs.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://luz.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://ebn.vqdsnc.cn

Ruby: arr.index(x)
来源：http://jhf.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://cql.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://ejj.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://miu.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://grr.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://tte.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://yvq.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pka.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://asg.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fvp.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://het.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://ajv.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zei.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ane.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://thg.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://mpu.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://ttn.havefunace.top

Go:   // 手写循环
来源：http://bow.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oak.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pdg.xylfe.cn

[D15] 去重
来源：http://mli.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jwb.0kj1m.cn

PHP:  array_unique($arr);
来源：http://fag.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://oxi.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://btm.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djr.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://snv.52xcode.cn

Ruby: arr.uniq
来源：http://xvk.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://pct.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://wqt.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mys.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://luz.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://abu.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfo.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://isu.zdqjudy.top

Go:   // 手写循环累加
来源：http://grp.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kty.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://din.zhixingplan.top

[D17] 最大值与最小值
来源：http://qxm.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://jxd.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://opo.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xle.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://rba.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dda.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xzf.yongpay.top

Ruby: arr.max;  arr.min
来源：http://heo.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://ggs.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://tgd.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oza.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://lps.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ijd.haohaochexian.top

TS:   nested.flat();
来源：http://oeo.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tru.hywenlv.cn

Go:   // 手写双层循环
来源：http://eqb.wangshuangyany.cn

Ruby: nested.flatten
来源：http://bqt.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wws.meibo888.top

[D19] 按字段分组
来源：http://uom.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rry.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mpi.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fvz.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rcw.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sor.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://xgx.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kqh.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tmh.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://bkv.hesvh.cn

Py:   Counter(arr)
来源：http://ovn.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://ara.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ktr.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tje.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eee.xuanzx.com

Go:   // 手写 map[T]int
来源：http://ley.vqdsnc.cn

Ruby: arr.tally
来源：http://vfw.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ldv.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://pff.sysykeji.top

Py:   x in arr
来源：http://nvz.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://fsv.zhixingplan.top

JS:   arr.includes(x)
来源：http://zkf.fengsongda.top

TS:   arr.includes(x)
来源：http://jrs.jqgufenzy.top

Java: list.contains(x)
来源：http://rsq.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://gbj.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://pup.zycfv.cn

C#:   list.Contains(x)
来源：http://trm.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://ruw.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ahe.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tty.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bjb.ctjpmb.com

TS:   [...arr];
来源：http://yqv.fktsv.cn

Java: new ArrayList<>(list);
来源：http://ssm.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://tfg.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://tzs.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://nil.52xcode.cn

[D23] reduce 累积计算
来源：http://fcw.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xrb.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zjj.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jke.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmj.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fuy.tian-w.cn

Go:   // 手写循环
来源：http://stg.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ssv.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gzz.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://gxd.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xij.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pxy.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kpp.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zvx.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rdl.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgw.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zza.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kdz.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://vzq.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hnd.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wjr.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jav.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kdb.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lte.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://izr.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://evv.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aop.cqqwz.cn

[D26] 数组转字符串
来源：http://iod.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://zal.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://lwa.tianlin.xyz

JS:   arr.join(", ")
来源：http://oxf.ivvv.top

TS:   arr.join(", ")
来源：http://isb.hywenlv.cn

Java: String.join(", ", list)
来源：http://doe.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://pqu.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://itp.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://lns.ehwqpu.com

================================================================================
来源：http://atx.andypj.xyz

E. 字符串处理
来源：http://emx.yj20258.top

================================================================================
来源：http://lqt.yonumen.top

[E01] 拼接字符串
来源：http://iwt.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://khp.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://syv.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqz.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://awg.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://smi.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qap.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qdh.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lev.dashuyun.cn

[E02] 重复字符串
来源：http://ykm.hfpthk.cn

Py:   "ab" * 3
来源：http://spt.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://thx.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://nev.ybcxt.top


<!-- 参考信息 -->