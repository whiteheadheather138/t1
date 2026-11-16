代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://kza.zhixingplan.top

C#:   using System.Text;
来源：http://ego.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://jai.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://dcm.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://lph.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://tfv.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://cfn.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ejv.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://ngs.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://kdi.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hfl.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://iwq.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ovc.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hmv.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zyy.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uuk.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://pat.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://oiz.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://flr.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://emk.ivvv.top

[C14] 泛型函数
来源：http://jtd.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://htm.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://egw.ctjpmb.com

JS:   // 无泛型
来源：http://chf.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xlb.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zcx.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cxz.hnqzz.top

Ruby: # 无泛型
来源：http://wjd.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wma.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://qgo.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vrx.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://twu.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xjv.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dci.jianghu66.top

Java: // 无解构
来源：http://seg.zhongyouzk.top

Go:   // 无解构
来源：http://tdr.kuanghao11.cn

Ruby: a, b = pair
来源：http://coe.havefunace.top

C#:   var (a, b) = pair;
来源：http://vey.ivvv.top

[C16] 函数 / 方法重载
来源：http://aki.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oiv.xylfe.cn

PHP:  // 无重载
来源：http://fqz.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sjw.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://xfm.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rml.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://ean.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://qbm.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bny.pengpengdd.cyou

================================================================================
来源：http://gtr.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://rmj.uphjek.com

================================================================================
来源：http://mcp.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://zci.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://obf.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lso.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dwk.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nhq.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pkq.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://yuy.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://qty.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dky.havefunace.top

[D02] 追加元素到末尾
来源：http://jky.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qnm.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qja.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://kus.c1oappe.top

TS:   arr.push(4);
来源：http://jpn.xylfe.cn

Java: list.add(4);
来源：http://jrq.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://ipc.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://kdo.fzhhl.top

C#:   list.Add(4);
来源：http://vej.yj20258888.top

[D03] 在指定位置插入元素
来源：http://utd.havefunace.top

Py:   arr.insert(0, 0)
来源：http://qea.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fnr.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cnr.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://hcm.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://wvu.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hpw.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jhd.cashguo.top

C#:   list.Insert(0, 0);
来源：http://tot.cqqwz.cn

[D04] 删除元素
来源：http://hib.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fpg.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rea.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://haj.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://zsw.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yti.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rpu.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xyl.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pme.hysaishi.cn

[D05] 访问与修改元素
来源：http://qpl.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wfp.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tob.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rmo.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://gtf.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://xha.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://yiy.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eau.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zuq.yfazqb.com

[D06] 数组长度
来源：http://lqj.snrcjt.cn

Py:   len(arr)
来源：http://jtq.tianlin.xyz

PHP:  count($arr);
来源：http://lcw.hywenlv.cn

JS:   arr.length
来源：http://mfh.xingfuxueyuan.xyz

TS:   arr.length
来源：http://ibc.zhiwuduotai.top

Java: list.size();
来源：http://aqz.xuanzx.com

Go:   len(arr)
来源：http://sll.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://uun.gotoacloud.top

C#:   list.Count;
来源：http://xaj.hcnkem.com

[D07] 切片 / 取子数组
来源：http://nay.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tst.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jxg.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://mzq.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://xmf.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://iac.birdmap.top

Go:   arr[1:4]
来源：http://hea.uphjek.com

Ruby: arr[1, 3]
来源：http://jei.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://ikg.daria6918.cn

[D08] 合并两个数组
来源：http://nyp.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://fmm.yj20258.top

PHP:  array_merge($a, $b);
来源：http://rzv.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vnx.tarul.cn

TS:   [...a, ...b];
来源：http://bma.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vcx.zhongyouzk.top

Go:   append(a, b...)
来源：http://xme.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://ffz.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://zzu.fengsongda.top

[D09] 排序（升序）
来源：http://rur.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://zhl.9152youxi.cn

PHP:  sort($arr);
来源：http://bcv.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tbj.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hsc.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rtr.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nkd.snrcjt.cn

Ruby: arr.sort
来源：http://xur.bbcook.cn

C#:   list.Sort();
来源：http://pwi.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://olm.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dzt.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqo.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ydw.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ajh.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rgc.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fgf.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnq.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://klq.jinqigufen.top

[D11] 反转数组
来源：http://kth.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yvw.guannengcc.top

PHP:  array_reverse($arr);
来源：http://lqu.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mik.hammf.cn

TS:   [...arr].reverse();
来源：http://ivb.fktsv.cn

Java: Collections.reverse(list);
来源：http://ftl.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://rwc.hnxiangtu.top

Ruby: arr.reverse
来源：http://bdl.xylfe.cn

C#:   list.Reverse();
来源：http://hot.sxryk.cn

[D12] 查找元素下标
来源：http://trh.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://qqa.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tzo.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nhl.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xkz.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xzn.cashguo.top

Go:   slices.Index(arr, x)
来源：http://ujs.zhixingplan.top

Ruby: arr.index(x)
来源：http://sum.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://pyh.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://mag.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yei.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ldv.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://lzr.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://shb.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ozs.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jgy.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://fem.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nfu.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://fik.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mgx.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybo.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://ewn.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://pdz.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwt.feifeiyinyue.top

Go:   // 手写循环
来源：http://rip.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://oph.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fqw.ctjpmb.com

[D15] 去重
来源：http://ozk.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gwk.nanxinkj.top

PHP:  array_unique($arr);
来源：http://hyt.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://krq.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://ilk.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dnn.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://smz.yangfankeji.com

Ruby: arr.uniq
来源：http://wbv.yonumen.top

C#:   list.Distinct().ToList()
来源：http://vbd.nanxinkj.top

[D16] 求和与平均值
来源：http://xtq.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://flg.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xev.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqt.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rvx.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nda.zhongyouzk.top

Go:   // 手写循环累加
来源：http://oei.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zhn.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://xuy.wangdashe.top

[D17] 最大值与最小值
来源：http://bqw.birdmap.top

Py:   max(arr);  min(arr)
来源：http://qwp.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://udl.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gyy.havefunace.top

TS:   Math.max(...arr);
来源：http://ejd.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jxw.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oqt.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://yyd.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://tfj.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://fzj.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kwa.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://lso.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vch.iojbl.cn

TS:   nested.flat();
来源：http://yyj.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cnr.chenlongwang.top

Go:   // 手写双层循环
来源：http://vvx.fzhhl.top

Ruby: nested.flatten
来源：http://tcl.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vqd.snrcjt.cn

[D19] 按字段分组
来源：http://sre.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://djf.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xbj.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czp.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://ele.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jgd.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://bol.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yws.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://krg.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://qzv.yvedp.cn

Py:   Counter(arr)
来源：http://vtb.gzhubu.top

PHP:  array_count_values($arr);
来源：http://pix.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ddg.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cap.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sfd.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://qzx.jinqigufen.top

Ruby: arr.tally
来源：http://sij.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dbb.fehbvm.com

[D21] 判断是否包含某元素
来源：http://smm.jiagoushi.top

Py:   x in arr
来源：http://vac.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://epo.ydjk.org.cn

JS:   arr.includes(x)
来源：http://hge.gzhubu.top

TS:   arr.includes(x)
来源：http://owu.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://epu.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://pzn.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://gyv.bbcook.cn

C#:   list.Contains(x)
来源：http://ylh.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://yzk.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ymx.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ome.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nfr.pycfn.com

TS:   [...arr];
来源：http://eux.hcnkem.com

Java: new ArrayList<>(list);
来源：http://sga.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://byr.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://pwu.yongpay.top

C#:   new List<int>(list);
来源：http://kek.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://tzv.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qlb.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mfs.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yur.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svz.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hkv.gzhubu.top

Go:   // 手写循环
来源：http://zri.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://znz.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ngp.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://tbs.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rgn.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nya.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hmh.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lsr.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mey.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jog.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vdh.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kfv.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://lnb.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kpu.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kgd.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rwg.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zvg.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mqc.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mai.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gzu.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://clw.fengsongda.top

[D26] 数组转字符串
来源：http://zlr.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://vfm.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://wla.yfazqb.com

JS:   arr.join(", ")
来源：http://dzw.dashuyun.cn

TS:   arr.join(", ")
来源：http://opl.fzhhl.top

Java: String.join(", ", list)
来源：http://jnn.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://rdt.yuxming.cn

Ruby: arr.join(", ")
来源：http://plp.xuanzx.com

C#:   string.Join(", ", list)
来源：http://jfy.nwbrower.top

================================================================================
来源：http://tug.gogol.net.cn

E. 字符串处理
来源：http://zfn.haohaochexian.top

================================================================================
来源：http://xrp.tian-w.cn

[E01] 拼接字符串
来源：http://umo.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dar.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fdm.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mmq.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bxj.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://obw.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yct.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gxm.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qhy.dashuyun.cn

[E02] 重复字符串
来源：http://oms.gogol.net.cn

Py:   "ab" * 3
来源：http://pmq.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://pvk.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://rxs.zhiwuduotai.top


<!-- 参考信息 -->