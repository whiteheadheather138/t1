代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yau.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dri.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hkf.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwn.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://gcv.mhx1999.top

Go:   func add(a, b int) int
来源：http://rgt.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kwn.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jkd.yj20258888.top

[C14] 泛型函数
来源：http://rjh.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mzk.sufxvd.cn

PHP:  // 无泛型
来源：http://ozo.fktsv.cn

JS:   // 无泛型
来源：http://rbt.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aqu.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nxj.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://erb.shangyingyoupin.top

Ruby: # 无泛型
来源：http://cgq.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ara.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://vah.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vkn.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://sfw.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zxd.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xqj.nanxuanxn.top

Java: // 无解构
来源：http://rny.hnxiangtu.top

Go:   // 无解构
来源：http://ymp.nanxinkj.top

Ruby: a, b = pair
来源：http://wuq.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://fsw.tarul.cn

[C16] 函数 / 方法重载
来源：http://tiw.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hrm.birdmap.top

PHP:  // 无重载
来源：http://nsj.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://oze.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://ysz.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gra.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://ppa.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://glk.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xpk.vehdjk.com

================================================================================
来源：http://mzt.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://bgn.shzxlz.cn

================================================================================
来源：http://kbg.52xcode.cn

[D01] 创建数组 / 列表
来源：http://dpg.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vwx.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xac.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oso.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://axw.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pkq.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://vqr.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://gjp.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://phr.daxiang520.top

[D02] 追加元素到末尾
来源：http://rec.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bfr.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zkr.zycfv.cn

JS:   arr.push(4);
来源：http://jnb.yueranfly.top

TS:   arr.push(4);
来源：http://qbf.fehbvm.com

Java: list.add(4);
来源：http://yfj.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://ulm.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://cxb.yj202588.top

C#:   list.Add(4);
来源：http://pug.yueranfly.top

[D03] 在指定位置插入元素
来源：http://zci.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://vip.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zyz.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ljq.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://mwx.hywenlv.cn

Java: list.add(0, 0);
来源：http://plw.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://xca.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nhv.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://krd.zhixingplan.top

[D04] 删除元素
来源：http://fqx.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jme.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ues.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lla.tanke756.top

TS:   arr.splice(0, 1);
来源：http://efi.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqi.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://taz.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mkc.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://prs.aizwys.cn

[D05] 访问与修改元素
来源：http://izw.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fsa.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qxg.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uva.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://oxz.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://zbh.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://uqj.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tos.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ebr.zhongyouzk.top

[D06] 数组长度
来源：http://xge.jinqigufen.top

Py:   len(arr)
来源：http://pgp.cdnleiting.top

PHP:  count($arr);
来源：http://jdy.meibo888.top

JS:   arr.length
来源：http://pjc.chenlongwang.top

TS:   arr.length
来源：http://fuc.yonumen.top

Java: list.size();
来源：http://lyu.jinyuanbaomall.cn

Go:   len(arr)
来源：http://kbq.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://uqv.aibaodan.cn

C#:   list.Count;
来源：http://pgu.316326.xyz

[D07] 切片 / 取子数组
来源：http://sge.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ydy.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yox.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://vha.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://nsx.svipenyu.cn

Java: list.subList(1, 4);
来源：http://omg.yueranfly.top

Go:   arr[1:4]
来源：http://tcs.andypj.xyz

Ruby: arr[1, 3]
来源：http://sbr.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://rri.jqgufenzy.top

[D08] 合并两个数组
来源：http://fxp.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://ytq.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://udb.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://auz.zycfv.cn

TS:   [...a, ...b];
来源：http://spc.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://its.yvedp.cn

Go:   append(a, b...)
来源：http://hfy.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://iwi.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://bkr.jinqigufen.top

[D09] 排序（升序）
来源：http://stu.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://tps.cqqwz.cn

PHP:  sort($arr);
来源：http://bxs.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ugu.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://twt.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://otm.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nkg.jinqigfzy.top

Ruby: arr.sort
来源：http://nfb.shanyushiyangtech.top

C#:   list.Sort();
来源：http://erd.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwv.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nrz.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rpa.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fmx.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ypq.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://olo.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ybi.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://itw.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eqo.iojbl.cn

[D11] 反转数组
来源：http://mdz.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vao.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://lxd.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yww.zhixingplan.top

TS:   [...arr].reverse();
来源：http://djc.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://san.uphjek.com

Go:   slices.Reverse(arr)
来源：http://rqr.yj20258.top

Ruby: arr.reverse
来源：http://lgi.daria6918.cn

C#:   list.Reverse();
来源：http://uah.aizwys.cn

[D12] 查找元素下标
来源：http://jyc.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://tcg.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bra.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpw.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kav.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xbd.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://nyi.0kj1m.cn

Ruby: arr.index(x)
来源：http://reg.uphjek.com

C#:   list.IndexOf(x);
来源：http://yyo.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://ajy.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vrd.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cly.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://qmn.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://rmx.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ykp.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ddf.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sda.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wzq.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://jzd.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rtc.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ywp.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://eyp.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://tbn.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qiq.hongshengwenyu.top

Go:   // 手写循环
来源：http://azk.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pnp.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://soq.shzxlz.cn

[D15] 去重
来源：http://cmw.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://njb.daria6918.cn

PHP:  array_unique($arr);
来源：http://xab.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://cmm.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://mxh.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://puw.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jyc.yj202588.top

Ruby: arr.uniq
来源：http://fdi.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://hfp.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://oof.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ony.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dmi.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpi.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhz.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yud.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://zjt.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wxv.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://hpm.sysykeji.top

[D17] 最大值与最小值
来源：http://tbe.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://ksf.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://jdj.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fgz.zycfv.cn

TS:   Math.max(...arr);
来源：http://eev.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pqe.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kux.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://zxq.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://neu.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://zkr.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lpt.316326.xyz

PHP:  array_merge(...$nested);
来源：http://hnx.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ssy.uphjek.com

TS:   nested.flat();
来源：http://ppz.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://njz.hysaishi.cn

Go:   // 手写双层循环
来源：http://oqf.yfazqb.com

Ruby: nested.flatten
来源：http://eaz.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jdg.dashuyun.cn

[D19] 按字段分组
来源：http://wvd.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rcm.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jhh.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fgn.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ylb.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aab.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://dya.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://acd.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://azb.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://wxk.hammf.cn

Py:   Counter(arr)
来源：http://sex.daria6918.cn

PHP:  array_count_values($arr);
来源：http://kbr.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtz.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mcb.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mzq.epnwcf.com

Go:   // 手写 map[T]int
来源：http://nxi.xziqi.cn

Ruby: arr.tally
来源：http://hfo.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufl.mhx1999.top

[D21] 判断是否包含某元素
来源：http://nzw.ywan-chungtsiang.top

Py:   x in arr
来源：http://mqm.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://avz.vehdjk.com

JS:   arr.includes(x)
来源：http://aov.daria6918.cn

TS:   arr.includes(x)
来源：http://syk.xziqi.cn

Java: list.contains(x)
来源：http://lwk.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://abc.zdqjudy.top

Ruby: arr.include?(x)
来源：http://trl.sysykeji.top

C#:   list.Contains(x)
来源：http://srg.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://xmd.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dxz.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://egc.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lfz.shangyingyoupin.top

TS:   [...arr];
来源：http://zpi.ivvv.top

Java: new ArrayList<>(list);
来源：http://ikm.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://qhr.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://sya.ehwqpu.com

C#:   new List<int>(list);
来源：http://dru.gotoacloud.top

[D23] reduce 累积计算
来源：http://rnj.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://egc.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vig.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dmg.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zhj.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qvs.aibaodan.cn

Go:   // 手写循环
来源：http://aub.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lgh.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xcn.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://ias.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hyy.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ume.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijk.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dad.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ywl.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uxw.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kas.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uij.meibo888.top

[D25] Set 集合去重与交并差
来源：http://elq.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uhm.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fed.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oya.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hgg.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dyp.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://piw.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pvw.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qvf.cucudq.cn

[D26] 数组转字符串
来源：http://aon.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://veu.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://ssb.dashuyun.cn

JS:   arr.join(", ")
来源：http://mbu.vehdjk.com

TS:   arr.join(", ")
来源：http://uuf.tianlin.xyz

Java: String.join(", ", list)
来源：http://fkn.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ual.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://ewb.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://zrw.hcnkem.com

================================================================================
来源：http://czp.sysykeji.top

E. 字符串处理
来源：http://aiq.fktsv.cn

================================================================================
来源：http://qgc.gaohongyu789.top

[E01] 拼接字符串
来源：http://hps.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jrf.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://alt.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://stw.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://str.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rmq.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ril.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ahj.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vez.tarul.cn

[E02] 重复字符串
来源：http://uly.fzhhl.top

Py:   "ab" * 3
来源：http://yfi.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://dae.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://imr.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://ajb.yuanzhike.top

Java: "ab".repeat(3)
来源：http://uey.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://naj.yj202588.top

Ruby: "ab" * 3
来源：http://imp.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://peo.chenlongwang.top

[E03] 截取子串
来源：http://tfc.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hua.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iis.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ulj.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://opd.epnwcf.com

Java: s.substring(1, 4)
来源：http://rff.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cso.ppjwa.cn


<!-- 参考信息 -->