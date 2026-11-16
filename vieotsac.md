代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gtl.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzy.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zdy.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nko.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://dij.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://xwx.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mvr.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dnu.gogol.net.cn

[C14] 泛型函数
来源：http://lii.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gsi.ybcxt.top

PHP:  // 无泛型
来源：http://ftc.svipenyu.cn

JS:   // 无泛型
来源：http://jhz.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ksn.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jjh.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rdw.zycfv.cn

Ruby: # 无泛型
来源：http://ebu.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kln.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://ter.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://liw.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://kps.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qny.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fta.nwbrower.top

Java: // 无解构
来源：http://jrr.jqgufenzy.top

Go:   // 无解构
来源：http://exb.ydzc1.top

Ruby: a, b = pair
来源：http://sxm.fzhhl.top

C#:   var (a, b) = pair;
来源：http://jer.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://axw.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryk.hnxiangtu.top

PHP:  // 无重载
来源：http://ljk.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lbc.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ukn.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://nwl.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://xet.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://cgk.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nbx.bbcook.cn

================================================================================
来源：http://wsa.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://iiy.daria6918.cn

================================================================================
来源：http://irb.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://dcs.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://dkr.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cci.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vqf.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wrr.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://huz.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://abq.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://eej.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oto.sweek.top

[D02] 追加元素到末尾
来源：http://ggo.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mqo.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xzs.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://mqt.jqgufenzy.top

TS:   arr.push(4);
来源：http://pmg.havefunace.top

Java: list.add(4);
来源：http://ltn.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://goq.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://yxy.mhx1999.top

C#:   list.Add(4);
来源：http://foj.xinyue.icu

[D03] 在指定位置插入元素
来源：http://puy.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://yet.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nxx.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cnl.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://dvk.sjlbkw.cn

Java: list.add(0, 0);
来源：http://jyd.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://yyn.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bmi.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://ryy.yj20258.top

[D04] 删除元素
来源：http://rmr.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyx.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mnc.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://epw.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://ilk.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://enl.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yaa.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wtq.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ysc.daxiang520.top

[D05] 访问与修改元素
来源：http://jpk.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://omi.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ert.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ayh.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://mmh.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://jpz.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://oyb.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gzo.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zec.jinqigufen.top

[D06] 数组长度
来源：http://nwh.bbcook.cn

Py:   len(arr)
来源：http://hho.gotoacloud.top

PHP:  count($arr);
来源：http://bdb.kuanghao11.cn

JS:   arr.length
来源：http://cgr.gzhubu.top

TS:   arr.length
来源：http://wyn.jinyuanbaomall.cn

Java: list.size();
来源：http://kkx.c1oappe.top

Go:   len(arr)
来源：http://dzl.gzhubu.top

Ruby: arr.length; arr.size
来源：http://pug.jinyuanbaomall.cn

C#:   list.Count;
来源：http://rid.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://les.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rul.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sbk.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://dnp.316326.xyz

TS:   arr.slice(1, 4);
来源：http://llv.uphjek.com

Java: list.subList(1, 4);
来源：http://rqf.zhiwuduotai.top

Go:   arr[1:4]
来源：http://ffv.gzhubu.top

Ruby: arr[1, 3]
来源：http://iar.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://mjd.epnwcf.com

[D08] 合并两个数组
来源：http://yld.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://uqw.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://tgq.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rkp.yonumen.top

TS:   [...a, ...b];
来源：http://awu.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vrw.bbcook.cn

Go:   append(a, b...)
来源：http://mas.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://eev.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://sqs.jyoumei.cn

[D09] 排序（升序）
来源：http://nuq.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://krq.fehbvm.com

PHP:  sort($arr);
来源：http://bjp.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://phd.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tdl.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bcn.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yot.epnwcf.com

Ruby: arr.sort
来源：http://cvx.tianlin.xyz

C#:   list.Sort();
来源：http://vax.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bei.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jxw.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vvw.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sxh.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwx.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vpq.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://erg.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xun.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ieq.wangshuangyany.cn

[D11] 反转数组
来源：http://ckg.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qub.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://dpg.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sqd.guannengcc.top

TS:   [...arr].reverse();
来源：http://xyq.ehwqpu.com

Java: Collections.reverse(list);
来源：http://gle.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://ere.fktsv.cn

Ruby: arr.reverse
来源：http://aam.yuxming.cn

C#:   list.Reverse();
来源：http://him.uphjek.com

[D12] 查找元素下标
来源：http://mad.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://kzb.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://loe.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://srl.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://guf.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://won.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://urj.hnxiangtu.top

Ruby: arr.index(x)
来源：http://nxm.tanke756.top

C#:   list.IndexOf(x);
来源：http://vxp.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://biw.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://djy.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ujn.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://fjj.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://qnv.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://acy.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fsq.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://ivz.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wng.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://lbg.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xez.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iwq.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://hjf.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://nvy.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ldg.sufxvd.cn

Go:   // 手写循环
来源：http://buz.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fmt.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://upv.zhengqikj.top

[D15] 去重
来源：http://cou.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tkq.aibaodan.cn

PHP:  array_unique($arr);
来源：http://wjm.daxiang520.top

JS:   [...new Set(arr)]
来源：http://iay.tian-w.cn

TS:   [...new Set(arr)]
来源：http://evt.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uuz.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://ewe.cheryme.top

Ruby: arr.uniq
来源：http://gyn.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://tjo.sxryk.cn

[D16] 求和与平均值
来源：http://kdd.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yao.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jgu.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xrb.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ala.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ajp.zhixingplan.top

Go:   // 手写循环累加
来源：http://hjl.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hbg.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://khd.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://hxm.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://vtq.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://yhk.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wth.svipenyu.cn

TS:   Math.max(...arr);
来源：http://tgz.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xsg.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oni.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://nqi.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://pxo.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://ygy.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zbe.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://dhf.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uow.jinqigfzy.top

TS:   nested.flat();
来源：http://iqy.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eej.yj202588.top

Go:   // 手写双层循环
来源：http://yxr.aibaodan.cn

Ruby: nested.flatten
来源：http://vkm.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dwj.hongshengwenyu.top

[D19] 按字段分组
来源：http://vxl.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xwx.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nvc.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lqu.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vov.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgr.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://yed.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://otb.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bxk.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://iqu.gogol.net.cn

Py:   Counter(arr)
来源：http://bak.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://rvd.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://enr.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://otg.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sff.yfazqb.com

Go:   // 手写 map[T]int
来源：http://dpl.hcnkem.com

Ruby: arr.tally
来源：http://ior.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wxj.vehdjk.com

[D21] 判断是否包含某元素
来源：http://uqs.sweek.top

Py:   x in arr
来源：http://ebk.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://sky.aizwys.cn

JS:   arr.includes(x)
来源：http://qfr.bbcook.cn

TS:   arr.includes(x)
来源：http://eus.nanxinkj.top

Java: list.contains(x)
来源：http://xgm.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://uzm.0kj1m.cn

Ruby: arr.include?(x)
来源：http://mln.jqgufenzy.top

C#:   list.Contains(x)
来源：http://lfq.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://qce.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://krz.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jdx.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cse.hysaishi.cn

TS:   [...arr];
来源：http://ril.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://aei.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://knr.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://cun.9152youxi.cn

C#:   new List<int>(list);
来源：http://unk.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://eke.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wxu.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://osw.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://umv.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkz.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdm.wangdashe.top

Go:   // 手写循环
来源：http://mpw.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eoe.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pqw.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://oxx.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfv.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dct.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://shd.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://byp.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eml.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bic.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://itj.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nzi.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://abd.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kqu.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yuh.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sau.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qep.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hny.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kaz.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://luy.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kyq.gzhubu.top

[D26] 数组转字符串
来源：http://djq.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://uoz.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://vsm.zdqjudy.top

JS:   arr.join(", ")
来源：http://nhn.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://zng.sjlbkw.cn

Java: String.join(", ", list)
来源：http://vov.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://lwi.ctjpmb.com

Ruby: arr.join(", ")
来源：http://wva.xylfe.cn

C#:   string.Join(", ", list)
来源：http://ssc.zhixingplan.top

================================================================================
来源：http://kuf.zdqjudy.top

E. 字符串处理
来源：http://ega.feifeiyinyue.top

================================================================================
来源：http://wit.gzhubu.top

[E01] 拼接字符串
来源：http://nix.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lig.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqp.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxg.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nca.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://voc.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ben.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://toc.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jao.aizwys.cn

[E02] 重复字符串
来源：http://lrs.zdbjq.cn

Py:   "ab" * 3
来源：http://nbq.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://wgo.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://qwg.c1oappe.top

TS:   "ab".repeat(3)
来源：http://jkp.cqqwz.cn

Java: "ab".repeat(3)
来源：http://zvv.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://zcz.dashuyun.cn

Ruby: "ab" * 3
来源：http://izf.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfa.zhixingplan.top

[E03] 截取子串
来源：http://suy.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dng.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uvm.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bmn.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://qgq.daria6918.cn

Java: s.substring(1, 4)
来源：http://nkb.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uai.yj20258888.top


<!-- 参考信息 -->