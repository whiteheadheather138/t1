代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://vih.yj202588.top

C#:   using System.Text;
来源：http://sms.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://zfp.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://fos.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://ovb.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://izu.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://wdc.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hji.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://tip.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://crl.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xlq.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://fzy.yuxming.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://plg.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlj.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jhs.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvj.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://hfu.ehwqpu.com

Go:   func add(a, b int) int
来源：http://kvf.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zts.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://tjz.daxiang520.top

[C14] 泛型函数
来源：http://fwt.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uhm.chenlongwang.top

PHP:  // 无泛型
来源：http://dje.iojbl.cn

JS:   // 无泛型
来源：http://vvu.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eij.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gou.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obd.daxiang520.top

Ruby: # 无泛型
来源：http://jpf.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wnd.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://fik.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fzm.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://xdq.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zay.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gdk.cheryme.top

Java: // 无解构
来源：http://zga.yanxiufei.cn

Go:   // 无解构
来源：http://cuz.shzxlz.cn

Ruby: a, b = pair
来源：http://xxm.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://xvg.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://apm.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://otg.jinghuilouyu.cn

PHP:  // 无重载
来源：http://ura.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gej.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://akp.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://koq.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://vkp.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://xco.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://awx.chenjidiqi.icu

================================================================================
来源：http://tdw.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://kfe.bjfxy.top

================================================================================
来源：http://azf.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://spl.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yrb.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bbo.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ckw.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgy.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wmj.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://oyd.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://pim.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kue.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://hnf.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rem.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yjt.shzxlz.cn

JS:   arr.push(4);
来源：http://pkd.hnqzz.top

TS:   arr.push(4);
来源：http://pth.feifeiyinyue.top

Java: list.add(4);
来源：http://ljo.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://ppp.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ykx.xinyue.icu

C#:   list.Add(4);
来源：http://vai.hammf.cn

[D03] 在指定位置插入元素
来源：http://ifr.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://oyb.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ckw.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rxx.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://jjs.chenzaomai.com

Java: list.add(0, 0);
来源：http://iar.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://skr.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uvz.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://gzu.zhongyouzk.top

[D04] 删除元素
来源：http://yha.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://caw.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fur.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ylv.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://vcu.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hre.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tti.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qnp.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uim.sweek.top

[D05] 访问与修改元素
来源：http://puf.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mqm.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://buo.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://szb.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://jdm.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://phz.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://tiq.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ktd.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dlk.zycfv.cn

[D06] 数组长度
来源：http://xeb.redwolf501.top

Py:   len(arr)
来源：http://dmi.yuxming.cn

PHP:  count($arr);
来源：http://jpz.yuxming.cn

JS:   arr.length
来源：http://uct.guannengcc.top

TS:   arr.length
来源：http://prd.fzhhl.top

Java: list.size();
来源：http://ohh.xinyue.icu

Go:   len(arr)
来源：http://zps.316326.xyz

Ruby: arr.length; arr.size
来源：http://xgt.hysaishi.cn

C#:   list.Count;
来源：http://rmy.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://ile.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tuh.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://urh.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://cak.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://kty.tianlin.xyz

Java: list.subList(1, 4);
来源：http://cxy.yangfankeji.com

Go:   arr[1:4]
来源：http://jvw.ehwqpu.com

Ruby: arr[1, 3]
来源：http://gxj.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://dum.pycfn.com

[D08] 合并两个数组
来源：http://vni.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://dez.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://gpd.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uis.guowangkeji.top

TS:   [...a, ...b];
来源：http://vrz.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mrk.shuidangran.top

Go:   append(a, b...)
来源：http://vgu.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://lfs.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://jwi.xuanzx.com

[D09] 排序（升序）
来源：http://qec.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ofk.birdmap.top

PHP:  sort($arr);
来源：http://yqa.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hzb.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://inq.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://rzj.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vax.hysaishi.cn

Ruby: arr.sort
来源：http://aiz.kuanghao11.cn

C#:   list.Sort();
来源：http://mll.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://opv.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xak.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sgc.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zip.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sle.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tyo.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://orx.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqf.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qye.sxryk.cn

[D11] 反转数组
来源：http://tll.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://lpi.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://zqo.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vic.epnwcf.com

TS:   [...arr].reverse();
来源：http://bsk.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://dzn.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://wvv.ehwqpu.com

Ruby: arr.reverse
来源：http://dcx.jqgfzy.top

C#:   list.Reverse();
来源：http://prp.cheryme.top

[D12] 查找元素下标
来源：http://zyk.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://nbt.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rrs.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecr.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihn.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nbh.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://vwg.hfpthk.cn

Ruby: arr.index(x)
来源：http://knn.hesvh.cn

C#:   list.IndexOf(x);
来源：http://hxk.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://kcv.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rer.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cca.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://zha.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://pjg.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xfr.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pcf.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jpe.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qgv.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://bgi.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://foc.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://akm.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://fip.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://ptq.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ayj.hammf.cn

Go:   // 手写循环
来源：http://grj.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://sya.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://cdo.guannengcc.top

[D15] 去重
来源：http://obp.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://khj.hammf.cn

PHP:  array_unique($arr);
来源：http://cpd.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://lho.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://gqp.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vnx.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lud.chenlongwang.top

Ruby: arr.uniq
来源：http://waf.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://teq.ydzc1.top

[D16] 求和与平均值
来源：http://tbs.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uzq.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zds.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgp.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://izm.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vfx.xylfe.cn

Go:   // 手写循环累加
来源：http://uoj.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wcb.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://yzz.0kj1m.cn

[D17] 最大值与最小值
来源：http://nvr.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://jlm.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://kek.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pae.dianchejie.cn

TS:   Math.max(...arr);
来源：http://jnf.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vhb.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgx.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://ztb.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://jaq.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://omb.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nrl.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://qub.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ejz.jianghu66.top

TS:   nested.flat();
来源：http://ufr.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jyk.gzhubu.top

Go:   // 手写双层循环
来源：http://jrv.haohaochexian.top

Ruby: nested.flatten
来源：http://ncb.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kvn.haohaochexian.top

[D19] 按字段分组
来源：http://bkw.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxb.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vab.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nug.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lao.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xnk.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://giu.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ttl.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bkk.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://iso.hongshengwenyu.top

Py:   Counter(arr)
来源：http://gte.bbcook.cn

PHP:  array_count_values($arr);
来源：http://hkt.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wym.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cug.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://igo.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://wdv.cashguo.top

Ruby: arr.tally
来源：http://mdk.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eee.bbcook.cn

[D21] 判断是否包含某元素
来源：http://xnv.nanxuanxn.top

Py:   x in arr
来源：http://wxt.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://ewx.hfpthk.cn

JS:   arr.includes(x)
来源：http://mkt.cheryme.top

TS:   arr.includes(x)
来源：http://boy.zhongyouzk.top

Java: list.contains(x)
来源：http://rmq.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://bfi.tianlin.xyz

Ruby: arr.include?(x)
来源：http://yyw.chenlongwang.top

C#:   list.Contains(x)
来源：http://lmh.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://avn.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vcy.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rng.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eke.ivvv.top

TS:   [...arr];
来源：http://mvq.daria6918.cn

Java: new ArrayList<>(list);
来源：http://pew.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://xln.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://fye.ivvv.top

C#:   new List<int>(list);
来源：http://sbe.hnxiangtu.top

[D23] reduce 累积计算
来源：http://vct.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hcy.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cum.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jzd.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tip.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://imp.cheryme.top

Go:   // 手写循环
来源：http://dcb.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gix.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tiw.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://tpu.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jkw.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ubz.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://juj.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ipq.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnu.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cgr.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wcn.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wbr.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://als.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zyr.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kyq.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yft.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xuj.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fjc.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dbb.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ghz.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtw.hesvh.cn

[D26] 数组转字符串
来源：http://uaa.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://oou.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://irr.jianghu66.top

JS:   arr.join(", ")
来源：http://ili.yvedp.cn

TS:   arr.join(", ")
来源：http://duo.fengsongda.top

Java: String.join(", ", list)
来源：http://kou.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://xbu.ctjpmb.com

Ruby: arr.join(", ")
来源：http://yrn.yj202588.top

C#:   string.Join(", ", list)
来源：http://mwz.yj202588.top

================================================================================
来源：http://sox.shanyushiyangtech.top

E. 字符串处理
来源：http://vbs.cashguo.top

================================================================================
来源：http://odr.tian-w.cn

[E01] 拼接字符串
来源：http://cdr.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ytd.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xlj.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzt.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qeh.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nzh.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ptw.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tmy.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://myg.52xcode.cn

[E02] 重复字符串
来源：http://yvl.sweek.top

Py:   "ab" * 3
来源：http://mcv.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://nxb.iojbl.cn

JS:   "ab".repeat(3)
来源：http://lfe.ppjwa.cn


<!-- 参考信息 -->