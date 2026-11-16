代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://cpu.kuanghao11.cn

C#:   using System.Text;
来源：http://zrn.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://cnk.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://dif.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://ojx.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://ied.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://pgj.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wnv.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://eqa.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://jxb.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dtd.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://yan.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tba.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vfq.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://npk.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqd.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://twx.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://fhv.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fet.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wfj.shuidangran.top

[C14] 泛型函数
来源：http://apa.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fcc.uphjek.com

PHP:  // 无泛型
来源：http://zdu.daria6918.cn

JS:   // 无泛型
来源：http://ioq.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://liq.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vjb.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ikh.shuidangran.top

Ruby: # 无泛型
来源：http://nzw.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uun.fktsv.cn

[C15] 解构 / 展开参数
来源：http://ung.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bme.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://gao.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gol.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hrc.chenlongwang.top

Java: // 无解构
来源：http://okm.dashuyun.cn

Go:   // 无解构
来源：http://muz.hfpthk.cn

Ruby: a, b = pair
来源：http://ypr.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://bnz.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://hex.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iwt.xylfe.cn

PHP:  // 无重载
来源：http://qeh.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vhr.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://bxw.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nzj.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://hgc.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://sjx.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hra.sjlbkw.cn

================================================================================
来源：http://oyp.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://aah.9152youxi.cn

================================================================================
来源：http://whr.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://err.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://bmb.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jvy.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://svq.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://tgo.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hdb.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://lcj.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://kta.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://maf.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://cso.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ocb.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lgp.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://vmv.dashuyun.cn

TS:   arr.push(4);
来源：http://tui.vqdsnc.cn

Java: list.add(4);
来源：http://wgy.meibo888.top

Go:   arr = append(arr, 4)
来源：http://dzi.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://iro.cheryme.top

C#:   list.Add(4);
来源：http://lcx.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://ygw.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://gku.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tcs.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wpj.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://lzo.andypj.xyz

Java: list.add(0, 0);
来源：http://hku.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xsu.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jnv.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://nmr.redwolf501.top

[D04] 删除元素
来源：http://jom.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wxc.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jqx.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nst.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://jdm.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fgd.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eed.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ivn.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lzh.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://tve.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qnh.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://swq.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cro.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://qlu.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://vno.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://grl.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rth.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bxv.yuanzhike.top

[D06] 数组长度
来源：http://iho.hcnkem.com

Py:   len(arr)
来源：http://xrc.316326.xyz

PHP:  count($arr);
来源：http://vcv.guannengcc.top

JS:   arr.length
来源：http://rjm.ybcxt.top

TS:   arr.length
来源：http://ree.shanyushiyangtech.top

Java: list.size();
来源：http://tdx.sweek.top

Go:   len(arr)
来源：http://bil.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://tpw.gaohongyu789.top

C#:   list.Count;
来源：http://spe.yj20258.top

[D07] 切片 / 取子数组
来源：http://arb.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pof.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://hjk.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://pbj.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://yyh.hesvh.cn

Java: list.subList(1, 4);
来源：http://pdy.zhixingplan.top

Go:   arr[1:4]
来源：http://yec.nanxinkj.top

Ruby: arr[1, 3]
来源：http://nfm.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://oic.yongpay.top

[D08] 合并两个数组
来源：http://ntz.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://tdu.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://lsz.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://brq.jyoumei.cn

TS:   [...a, ...b];
来源：http://xag.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dqa.haohaochexian.top

Go:   append(a, b...)
来源：http://iqo.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://zgr.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://gdx.sufxvd.cn

[D09] 排序（升序）
来源：http://hjn.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://gah.birdmap.top

PHP:  sort($arr);
来源：http://cbn.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://niy.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://knw.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://udz.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://btu.zhongyouzk.top

Ruby: arr.sort
来源：http://lhf.ctjpmb.com

C#:   list.Sort();
来源：http://qbl.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://veq.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gzq.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yla.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mdu.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqi.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tkx.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uaq.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hmt.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jaw.daria6918.cn

[D11] 反转数组
来源：http://qwh.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://wmi.ivvv.top

PHP:  array_reverse($arr);
来源：http://pqg.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oym.jqgfzy.top

TS:   [...arr].reverse();
来源：http://pry.bbcook.cn

Java: Collections.reverse(list);
来源：http://pzd.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://amo.hongshengwenyu.top

Ruby: arr.reverse
来源：http://owj.smart0.xyz

C#:   list.Reverse();
来源：http://iqs.uphjek.com

[D12] 查找元素下标
来源：http://mmf.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://ffr.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uvn.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yae.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cih.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vph.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://lam.daxiang520.top

Ruby: arr.index(x)
来源：http://ktm.birdmap.top

C#:   list.IndexOf(x);
来源：http://yrq.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://csf.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kec.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wsh.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://fdw.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://lzt.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ref.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dqx.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://qii.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zhp.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://gzt.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vio.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sys.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://hmu.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://psv.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fgw.havefunace.top

Go:   // 手写循环
来源：http://nda.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jkf.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://bgj.jqgufenzy.top

[D15] 去重
来源：http://oml.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fux.guannengcc.top

PHP:  array_unique($arr);
来源：http://ghc.aizwys.cn

JS:   [...new Set(arr)]
来源：http://bwl.nwbrower.top

TS:   [...new Set(arr)]
来源：http://hoj.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ibt.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://ctq.tanke756.top

Ruby: arr.uniq
来源：http://mgp.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://anr.zhengqikj.top

[D16] 求和与平均值
来源：http://fpv.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bqc.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tkb.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://alu.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txh.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vzd.guowangkeji.top

Go:   // 手写循环累加
来源：http://kqd.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://exq.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://oib.chenzaomai.com

[D17] 最大值与最小值
来源：http://bpx.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://bll.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://mwr.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qyp.yj20258888.top

TS:   Math.max(...arr);
来源：http://mwu.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tjt.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ivm.meibo888.top

Ruby: arr.max;  arr.min
来源：http://sif.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://gtz.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://ewd.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xdc.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://nag.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://klc.zhiwuduotai.top

TS:   nested.flat();
来源：http://dsp.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qub.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://iou.feifeiyinyue.top

Ruby: nested.flatten
来源：http://sko.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qlk.haohaochexian.top

[D19] 按字段分组
来源：http://hnu.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ocy.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://azp.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rpj.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ouy.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oqy.cheryme.top

Go:   // 手写 map[string][]T
来源：http://hwb.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cgr.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vrj.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://svf.sweek.top

Py:   Counter(arr)
来源：http://bjj.yonumen.top

PHP:  array_count_values($arr);
来源：http://llu.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mti.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kge.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://clp.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://wyt.ydzc1.top

Ruby: arr.tally
来源：http://phu.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jfi.epnwcf.com

[D21] 判断是否包含某元素
来源：http://crk.daria6918.cn

Py:   x in arr
来源：http://tat.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://rjv.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://zxk.hesvh.cn

TS:   arr.includes(x)
来源：http://qgl.chenjidiqi.icu

Java: list.contains(x)
来源：http://iqc.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://fdv.xylfe.cn

Ruby: arr.include?(x)
来源：http://xgi.hnqzz.top

C#:   list.Contains(x)
来源：http://amo.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://rne.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://urg.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kqz.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pjx.iojbl.cn

TS:   [...arr];
来源：http://wwf.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://pom.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://tdj.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://tnf.zycfv.cn

C#:   new List<int>(list);
来源：http://slu.svipenyu.cn

[D23] reduce 累积计算
来源：http://hfd.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://asz.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxu.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsx.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://utt.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yhl.vehdjk.com

Go:   // 手写循环
来源：http://dsm.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bcp.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oss.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://mgr.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eid.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zfp.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hje.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dyx.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bgn.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tmp.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ehb.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ktb.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://pyz.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://par.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hwx.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://skq.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://huf.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bzl.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://svf.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iuk.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xyf.epnwcf.com

[D26] 数组转字符串
来源：http://xoh.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://gen.316326.xyz

PHP:  implode(", ", $arr);
来源：http://edl.hnqzz.top

JS:   arr.join(", ")
来源：http://kti.bjfxy.top

TS:   arr.join(", ")
来源：http://ani.guannengcc.top

Java: String.join(", ", list)
来源：http://bar.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://aet.ehwqpu.com

Ruby: arr.join(", ")
来源：http://fuy.tarul.cn

C#:   string.Join(", ", list)
来源：http://jbk.sweek.top

================================================================================
来源：http://jdb.yonumen.top

E. 字符串处理
来源：http://vnx.hesvh.cn

================================================================================
来源：http://wpx.uphjek.com

[E01] 拼接字符串
来源：http://nwd.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eec.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hdl.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iyz.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zio.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zxj.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uio.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://poo.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cjm.yongpay.top

[E02] 重复字符串
来源：http://dvc.yj20258.top

Py:   "ab" * 3
来源：http://aig.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://pao.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://iaz.uphjek.com


<!-- 参考信息 -->