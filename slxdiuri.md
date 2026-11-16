代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ygf.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ztp.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwj.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwn.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://avk.hesvh.cn

Go:   func add(a, b int) int
来源：http://ufc.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ocg.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pbd.zhengqikj.top

[C14] 泛型函数
来源：http://ofn.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lhn.vehdjk.com

PHP:  // 无泛型
来源：http://xdr.yuxming.cn

JS:   // 无泛型
来源：http://xcf.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://trw.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eur.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://awo.c1oappe.top

Ruby: # 无泛型
来源：http://cwn.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ypw.yuxming.cn

[C15] 解构 / 展开参数
来源：http://fov.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xhq.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://amj.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fss.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fix.jinghuilouyu.cn

Java: // 无解构
来源：http://lyv.snrcjt.cn

Go:   // 无解构
来源：http://ljh.nwbrower.top

Ruby: a, b = pair
来源：http://vbw.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://tdh.iojbl.cn

[C16] 函数 / 方法重载
来源：http://xxl.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qbu.jianghu66.top

PHP:  // 无重载
来源：http://yth.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pab.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://baa.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iom.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://cat.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://aik.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zwg.svipenyu.cn

================================================================================
来源：http://flx.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://qoe.guannengcc.top

================================================================================
来源：http://lvt.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://qel.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ntt.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vlq.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://chh.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdi.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gnz.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://iyq.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://bdh.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jkv.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://zwo.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://guq.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kyc.jqgufenzy.top

JS:   arr.push(4);
来源：http://nxx.vqdsnc.cn

TS:   arr.push(4);
来源：http://vns.jyoumei.cn

Java: list.add(4);
来源：http://yaw.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://kej.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://esf.9152youxi.cn

C#:   list.Add(4);
来源：http://qsr.yfazqb.com

[D03] 在指定位置插入元素
来源：http://aac.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://wsr.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lho.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qma.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://eno.yonumen.top

Java: list.add(0, 0);
来源：http://nlo.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fwi.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gfk.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://gnx.shanyushiyangtech.top

[D04] 删除元素
来源：http://ujf.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://phi.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eas.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hhx.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://ajr.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qnm.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hyy.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wmb.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eip.sysykeji.top

[D05] 访问与修改元素
来源：http://odi.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lns.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bdd.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mih.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://dhc.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://vuc.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://oxp.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oyv.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kck.redwolf501.top

[D06] 数组长度
来源：http://ksu.yanxiufei.cn

Py:   len(arr)
来源：http://bit.jyoumei.cn

PHP:  count($arr);
来源：http://ecm.aibaodan.cn

JS:   arr.length
来源：http://kxs.sjlbkw.cn

TS:   arr.length
来源：http://mfu.shuidangran.top

Java: list.size();
来源：http://qhe.aizwys.cn

Go:   len(arr)
来源：http://ffm.fktsv.cn

Ruby: arr.length; arr.size
来源：http://vkc.sjlbkw.cn

C#:   list.Count;
来源：http://qnb.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://vfn.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hdm.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qbm.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://lid.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://fnp.sxryk.cn

Java: list.subList(1, 4);
来源：http://pwy.sufxvd.cn

Go:   arr[1:4]
来源：http://mnd.sxryk.cn

Ruby: arr[1, 3]
来源：http://cxz.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://fcj.chenjidiqi.icu

[D08] 合并两个数组
来源：http://feu.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://bhl.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://umj.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rxb.fengsongda.top

TS:   [...a, ...b];
来源：http://cki.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wpe.meibo888.top

Go:   append(a, b...)
来源：http://byp.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://qyi.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://hpw.hnqzz.top

[D09] 排序（升序）
来源：http://zdk.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://xpp.svipenyu.cn

PHP:  sort($arr);
来源：http://bxi.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pcy.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpl.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hsf.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ymg.pengpengdd.cyou

Ruby: arr.sort
来源：http://uoi.52xcode.cn

C#:   list.Sort();
来源：http://raq.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tvi.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://njt.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyi.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cdk.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbw.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://adl.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rst.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://epj.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sju.zhixingplan.top

[D11] 反转数组
来源：http://cxb.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tgc.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://lgc.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cyx.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://oft.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://vjm.tanke756.top

Go:   slices.Reverse(arr)
来源：http://jpw.yuxming.cn

Ruby: arr.reverse
来源：http://pjy.aibaodan.cn

C#:   list.Reverse();
来源：http://bwr.zhengqikj.top

[D12] 查找元素下标
来源：http://zfs.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://dgv.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbf.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogl.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kpu.smart0.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqu.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://bkq.kuanghao11.cn

Ruby: arr.index(x)
来源：http://ere.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://acq.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://trr.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sbs.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kbj.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://gmz.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://gkw.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vif.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bsi.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://vdh.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pae.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://zck.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eox.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://icz.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://fqn.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://ynx.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gsz.cdnleiting.top

Go:   // 手写循环
来源：http://pgs.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rry.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mzb.nanxuanxn.top

[D15] 去重
来源：http://qci.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tiw.cucudq.cn

PHP:  array_unique($arr);
来源：http://sih.cashguo.top

JS:   [...new Set(arr)]
来源：http://hrb.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://hdh.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oeg.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://pcm.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://gbv.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://mur.uphjek.com

[D16] 求和与平均值
来源：http://qew.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ucr.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zyz.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://syw.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://guv.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xbp.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://zmt.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rnx.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://dja.nwbrower.top

[D17] 最大值与最小值
来源：http://bgs.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://geh.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://nhd.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vqd.zhengqikj.top

TS:   Math.max(...arr);
来源：http://psv.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://cvj.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oxx.pycfn.com

Ruby: arr.max;  arr.min
来源：http://zxv.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://dcm.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://tir.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zgy.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://tor.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://icc.yueranfly.top

TS:   nested.flat();
来源：http://off.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://miq.pycfn.com

Go:   // 手写双层循环
来源：http://agl.ydjk.org.cn

Ruby: nested.flatten
来源：http://ftf.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fhm.hesvh.cn

[D19] 按字段分组
来源：http://gyr.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ien.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vcq.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gqv.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hck.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://isj.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://epy.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ytt.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gbu.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://adv.yangfankeji.com

Py:   Counter(arr)
来源：http://hah.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://epo.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://shj.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltd.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xbc.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://mzj.ivvv.top

Ruby: arr.tally
来源：http://opj.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jjq.hammf.cn

[D21] 判断是否包含某元素
来源：http://fla.gaohongyu789.top

Py:   x in arr
来源：http://rho.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://hty.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://oil.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://zfy.nwbrower.top

Java: list.contains(x)
来源：http://tzw.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://bly.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://war.yangfankeji.com

C#:   list.Contains(x)
来源：http://mkp.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://alh.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qts.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mmv.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ibe.cqqwz.cn

TS:   [...arr];
来源：http://kyi.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://odf.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tzc.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://okk.vehdjk.com

C#:   new List<int>(list);
来源：http://ozg.cheryme.top

[D23] reduce 累积计算
来源：http://nqk.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gvd.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://osy.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aav.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fgf.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://djb.jinqigfzy.top

Go:   // 手写循环
来源：http://dam.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iez.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fra.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://qkj.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ehv.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ycz.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iks.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jnx.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hru.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ccm.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mrr.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vgv.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://jhj.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pif.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cvg.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hmi.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://olg.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vwb.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xxo.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fvj.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwg.shangyingyoupin.top

[D26] 数组转字符串
来源：http://bpk.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://ogp.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://gak.yangfankeji.com

JS:   arr.join(", ")
来源：http://rjy.dianchejie.cn

TS:   arr.join(", ")
来源：http://ahv.xuanzx.com

Java: String.join(", ", list)
来源：http://ink.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://nob.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://mwb.guannengcc.top

C#:   string.Join(", ", list)
来源：http://dya.tianlin.xyz

================================================================================
来源：http://oyu.shangyingyoupin.top

E. 字符串处理
来源：http://yna.jqgfzy.top

================================================================================
来源：http://pxr.jiagoushi.top

[E01] 拼接字符串
来源：http://cqd.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eak.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://azn.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oid.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hvg.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mjc.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mpu.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ctq.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwa.hcnkem.com

[E02] 重复字符串
来源：http://hdc.chenlongwang.top

Py:   "ab" * 3
来源：http://euf.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://stc.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://tep.yuxming.cn

TS:   "ab".repeat(3)
来源：http://pmz.epnwcf.com

Java: "ab".repeat(3)
来源：http://hff.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bpg.ivvv.top

Ruby: "ab" * 3
来源：http://nwo.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://svl.9152youxi.cn

[E03] 截取子串
来源：http://vxk.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kmf.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://srv.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bdt.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://hbh.ydzc1.top

Java: s.substring(1, 4)
来源：http://kau.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tls.zdbjq.cn


<!-- 参考信息 -->