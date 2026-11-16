代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://lib.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://gaj.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xyx.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://xwf.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://deq.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpc.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gly.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsj.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://its.52xcode.cn

Go:   func add(a, b int) int
来源：http://jxi.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tyq.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://buu.cdnleiting.top

[C14] 泛型函数
来源：http://gqr.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ggd.sysykeji.top

PHP:  // 无泛型
来源：http://pfx.yvedp.cn

JS:   // 无泛型
来源：http://xgq.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uqu.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zrg.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jde.zhoulong.xyz

Ruby: # 无泛型
来源：http://jsd.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ykm.yj202588.top

[C15] 解构 / 展开参数
来源：http://jeb.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tcl.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://atp.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rip.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ffv.shanyushiyangtech.top

Java: // 无解构
来源：http://vkv.xuetiantiany.cn

Go:   // 无解构
来源：http://ekz.zhengqikj.top

Ruby: a, b = pair
来源：http://wsi.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://ybc.xuanzx.com

[C16] 函数 / 方法重载
来源：http://vld.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vgq.yanxiufei.cn

PHP:  // 无重载
来源：http://ldb.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tjq.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://hhz.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qzn.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://gkp.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://ydg.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wrb.yj20258888.top

================================================================================
来源：http://lgb.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://uie.yonumen.top

================================================================================
来源：http://lor.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://mtg.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://add.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qtb.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cjc.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lfc.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mlt.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://zuu.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://evo.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cnw.shuidangran.top

[D02] 追加元素到末尾
来源：http://jzj.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nqy.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ytb.hfpthk.cn

JS:   arr.push(4);
来源：http://ldm.vqdsnc.cn

TS:   arr.push(4);
来源：http://ubw.svipenyu.cn

Java: list.add(4);
来源：http://uqq.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://sxb.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://lmr.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://pnt.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://kvi.sweek.top

Py:   arr.insert(0, 0)
来源：http://tqz.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rbl.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfb.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://cix.52xcode.cn

Java: list.add(0, 0);
来源：http://org.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://vta.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gxt.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://urx.jyoumei.cn

[D04] 删除元素
来源：http://fcc.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wfd.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yxp.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fii.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://dja.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fpo.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eig.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zhx.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blt.pycfn.com

[D05] 访问与修改元素
来源：http://qlh.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xlb.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pnm.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ryg.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://spi.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://usa.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://ewq.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ync.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ozs.hywenlv.cn

[D06] 数组长度
来源：http://wuy.yangfankeji.com

Py:   len(arr)
来源：http://oei.pengpengdd.cyou

PHP:  count($arr);
来源：http://uap.gaohongyu789.top

JS:   arr.length
来源：http://onb.tianlin.xyz

TS:   arr.length
来源：http://epy.yj202588.top

Java: list.size();
来源：http://cwx.jinqigufen.top

Go:   len(arr)
来源：http://hld.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://ijs.hywenlv.cn

C#:   list.Count;
来源：http://zam.yj20258.top

[D07] 切片 / 取子数组
来源：http://qmt.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://keg.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ane.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://tcy.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://oqg.hysaishi.cn

Java: list.subList(1, 4);
来源：http://brk.birdmap.top

Go:   arr[1:4]
来源：http://mwl.fehbvm.com

Ruby: arr[1, 3]
来源：http://imw.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://wjg.gotoacloud.top

[D08] 合并两个数组
来源：http://jpz.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://muf.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://pso.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wgu.jlsjyb.cn

TS:   [...a, ...b];
来源：http://nge.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vpr.ydzc1.top

Go:   append(a, b...)
来源：http://yin.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://zzn.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://anm.tanke756.top

[D09] 排序（升序）
来源：http://nzo.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vef.haohaochexian.top

PHP:  sort($arr);
来源：http://skc.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lln.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://rem.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vso.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipx.xuanzx.com

Ruby: arr.sort
来源：http://npd.ehwqpu.com

C#:   list.Sort();
来源：http://yxr.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xhe.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xyr.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uqy.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aah.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wly.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rfc.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://abl.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtf.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dxk.yvedp.cn

[D11] 反转数组
来源：http://zpm.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aec.c1oappe.top

PHP:  array_reverse($arr);
来源：http://gah.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zad.dashuyun.cn

TS:   [...arr].reverse();
来源：http://ukh.sysykeji.top

Java: Collections.reverse(list);
来源：http://rfe.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://jaz.hammf.cn

Ruby: arr.reverse
来源：http://eoy.tian-w.cn

C#:   list.Reverse();
来源：http://jvz.gzhubu.top

[D12] 查找元素下标
来源：http://gkw.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://jes.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://huo.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crw.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://trs.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bcy.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://vso.jianghu66.top

Ruby: arr.index(x)
来源：http://slm.wangdashe.top

C#:   list.IndexOf(x);
来源：http://van.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://knm.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kcg.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hfc.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://jfs.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://ukg.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yft.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nrg.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://nzd.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bqd.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://psc.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lvg.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mft.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://neg.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://zqo.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kof.jinghuilouyu.cn

Go:   // 手写循环
来源：http://xbz.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ujp.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jab.yfazqb.com

[D15] 去重
来源：http://bgz.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uqs.ehwqpu.com

PHP:  array_unique($arr);
来源：http://tmh.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://xdm.tanke756.top

TS:   [...new Set(arr)]
来源：http://vky.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pwe.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://plx.tanke756.top

Ruby: arr.uniq
来源：http://qdg.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://icc.ivvv.top

[D16] 求和与平均值
来源：http://ets.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qgk.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://twr.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qod.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rbr.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jjm.smart0.xyz

Go:   // 手写循环累加
来源：http://zbb.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fcq.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://jej.andypj.xyz

[D17] 最大值与最小值
来源：http://fcx.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://kcl.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://eqw.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pby.yj20258.top

TS:   Math.max(...arr);
来源：http://kle.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lba.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mze.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://uvt.cashguo.top

C#:   list.Max();  list.Min()
来源：http://nha.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://ett.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://phn.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://fzs.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nrf.svipenyu.cn

TS:   nested.flat();
来源：http://hng.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zqi.hfpthk.cn

Go:   // 手写双层循环
来源：http://pfy.andypj.xyz

Ruby: nested.flatten
来源：http://jie.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xnc.ybcxt.top

[D19] 按字段分组
来源：http://ibj.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://prz.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bfa.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xpu.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lnw.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vgm.yongpay.top

Go:   // 手写 map[string][]T
来源：http://udk.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cbs.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tjz.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://jch.xinyue.icu

Py:   Counter(arr)
来源：http://uok.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://saw.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrx.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rkc.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://crl.yj202588.top

Go:   // 手写 map[T]int
来源：http://xnq.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://ugf.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lfa.daria6918.cn

[D21] 判断是否包含某元素
来源：http://zvb.daria6918.cn

Py:   x in arr
来源：http://obd.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://tim.aibaodan.cn

JS:   arr.includes(x)
来源：http://guj.wangdashe.top

TS:   arr.includes(x)
来源：http://cbx.snrcjt.cn

Java: list.contains(x)
来源：http://qdr.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://eho.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://cyb.jinqigufen.top

C#:   list.Contains(x)
来源：http://wse.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://awe.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dzu.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fqj.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xvp.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://kxy.hesvh.cn

Java: new ArrayList<>(list);
来源：http://qny.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://yjf.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://wyo.aibaodan.cn

C#:   new List<int>(list);
来源：http://aie.daria6918.cn

[D23] reduce 累积计算
来源：http://lxs.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fhd.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://loa.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mww.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyt.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zth.tianlin.xyz

Go:   // 手写循环
来源：http://azk.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fxk.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdl.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://jwm.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://atd.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ccq.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tjh.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ucg.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nog.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://agj.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fnn.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vwo.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://hol.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nlk.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xqn.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tdu.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zan.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dmc.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bbk.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://osh.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hpt.jinqigfzy.top

[D26] 数组转字符串
来源：http://hmi.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://xbb.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://nfn.sjlbkw.cn

JS:   arr.join(", ")
来源：http://qhi.havefunace.top

TS:   arr.join(", ")
来源：http://dsq.yangfankeji.com

Java: String.join(", ", list)
来源：http://fmk.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://ixk.chenlongwang.top

Ruby: arr.join(", ")
来源：http://rui.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://rxs.andypj.xyz

================================================================================
来源：http://lvf.cqqwz.cn

E. 字符串处理
来源：http://bzl.wangdashe.top

================================================================================
来源：http://rhm.jinqigfzy.top

[E01] 拼接字符串
来源：http://lxh.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uiw.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xlm.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dbg.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jld.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nci.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://siq.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://div.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxl.nanxuanxn.top

[E02] 重复字符串
来源：http://blt.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://dnd.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://dvb.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://icq.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://fyb.ehwqpu.com

Java: "ab".repeat(3)
来源：http://ecj.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://cmn.yuanzhike.top

Ruby: "ab" * 3
来源：http://fkz.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mts.ctjpmb.com

[E03] 截取子串
来源：http://lyi.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://goy.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mtz.jiagoushi.top


<!-- 参考信息 -->