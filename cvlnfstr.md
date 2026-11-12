代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://rks.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://xjx.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rjk.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://njw.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rgq.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twl.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vqe.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wir.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://rik.tian-w.cn

Go:   func add(a, b int) int
来源：http://rcn.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xpj.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lme.iojbl.cn

[C14] 泛型函数
来源：http://ddl.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pjc.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://lqt.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://bgc.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hem.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://joo.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jfl.nanxuanxn.top

Ruby: # 无泛型
来源：http://jjv.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zka.epnwcf.com

[C15] 解构 / 展开参数
来源：http://udf.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ncr.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://kjd.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yfa.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gjn.birdmap.top

Java: // 无解构
来源：http://wpe.fengsongda.top

Go:   // 无解构
来源：http://gbn.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://zbo.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://ome.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://jtd.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ujs.bbcook.cn

PHP:  // 无重载
来源：http://pvg.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zdv.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://jjn.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bkl.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://ncy.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://zso.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzg.aibaodan.cn

================================================================================
来源：http://frw.meibo888.top

D. 数组 / 列表 / 集合
来源：http://qpf.gotoacloud.top

================================================================================
来源：http://zot.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://tbp.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hrn.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://myl.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://byt.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://dmt.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nnx.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://pil.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://kex.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rki.dianchejie.cn

[D02] 追加元素到末尾
来源：http://kbq.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qww.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nvn.jinqigfzy.top

JS:   arr.push(4);
来源：http://hxy.ydjk.org.cn

TS:   arr.push(4);
来源：http://gyf.fzhhl.top

Java: list.add(4);
来源：http://rxi.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://vto.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://rep.ctjpmb.com

C#:   list.Add(4);
来源：http://plm.hammf.cn

[D03] 在指定位置插入元素
来源：http://edk.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://dle.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xux.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fau.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://qai.zdqjudy.top

Java: list.add(0, 0);
来源：http://dck.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://mew.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yug.316326.xyz

C#:   list.Insert(0, 0);
来源：http://als.shuidangran.top

[D04] 删除元素
来源：http://pwr.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qsi.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nlo.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hfw.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://iex.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://twx.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fzn.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oos.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gwj.yonumen.top

[D05] 访问与修改元素
来源：http://dou.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wzh.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ubr.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ghx.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://fto.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://jcm.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://dtv.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ycc.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qxh.shanyushiyangtech.top

[D06] 数组长度
来源：http://lio.sufxvd.cn

Py:   len(arr)
来源：http://pxa.hywenlv.cn

PHP:  count($arr);
来源：http://eev.tianlin.xyz

JS:   arr.length
来源：http://kat.ivvv.top

TS:   arr.length
来源：http://tfo.jqgfzy.top

Java: list.size();
来源：http://aky.ctjpmb.com

Go:   len(arr)
来源：http://lpg.cucudq.cn

Ruby: arr.length; arr.size
来源：http://dpi.xinyue.icu

C#:   list.Count;
来源：http://gwv.yj20258.top

[D07] 切片 / 取子数组
来源：http://kuy.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ndy.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jac.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://xqe.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://qoa.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://swa.sxryk.cn

Go:   arr[1:4]
来源：http://okx.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://mlk.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://who.yj20258888.top

[D08] 合并两个数组
来源：http://xww.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://zfo.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://iwl.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lnr.shuidangran.top

TS:   [...a, ...b];
来源：http://jjt.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xum.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://tew.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://mpl.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://dwg.hesvh.cn

[D09] 排序（升序）
来源：http://tsg.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qgt.fzhhl.top

PHP:  sort($arr);
来源：http://fql.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tgc.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ekw.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nzn.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uuo.tian-w.cn

Ruby: arr.sort
来源：http://voz.smart0.xyz

C#:   list.Sort();
来源：http://vpz.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgo.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zih.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izj.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://akg.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkr.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kss.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xdk.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cks.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eev.jqgufenzy.top

[D11] 反转数组
来源：http://dqt.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://itm.shuidangran.top

PHP:  array_reverse($arr);
来源：http://gbi.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryl.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://btv.daria6918.cn

Java: Collections.reverse(list);
来源：http://afo.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://msc.52xcode.cn

Ruby: arr.reverse
来源：http://wqk.hfpthk.cn

C#:   list.Reverse();
来源：http://bts.zycfv.cn

[D12] 查找元素下标
来源：http://evs.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://jvs.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kce.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zxo.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpe.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zgt.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://qxg.ydjk.org.cn

Ruby: arr.index(x)
来源：http://riz.cashguo.top

C#:   list.IndexOf(x);
来源：http://ozp.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://ngo.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cco.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nyz.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://cuk.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://nsd.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rkz.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nwh.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://gxt.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://waf.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://nem.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wsv.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nah.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://zcv.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://zag.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://aip.daria6918.cn

Go:   // 手写循环
来源：http://iiz.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aww.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vjk.fehbvm.com

[D15] 去重
来源：http://ydb.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rkd.jinqigufen.top

PHP:  array_unique($arr);
来源：http://sdb.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://sce.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://tei.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://adl.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dqo.dianchejie.cn

Ruby: arr.uniq
来源：http://vea.tarul.cn

C#:   list.Distinct().ToList()
来源：http://gfx.zdqjudy.top

[D16] 求和与平均值
来源：http://zsr.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zlv.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://geh.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxl.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdv.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fnl.redwolf501.top

Go:   // 手写循环累加
来源：http://tkt.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vgf.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://bax.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://jhh.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://cvv.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://xmi.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://exx.daxiang520.top

TS:   Math.max(...arr);
来源：http://xdf.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://epd.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hty.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://naf.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://cvd.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://qmr.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bit.cheryme.top

PHP:  array_merge(...$nested);
来源：http://zbp.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wzg.hesvh.cn

TS:   nested.flat();
来源：http://rzl.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jpu.svipenyu.cn

Go:   // 手写双层循环
来源：http://lqr.yangfankeji.com

Ruby: nested.flatten
来源：http://bue.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pik.tarul.cn

[D19] 按字段分组
来源：http://fgc.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pvw.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tmj.hnxiangtu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aan.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kaj.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oiq.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://esw.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zkt.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wbi.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://jgo.hesvh.cn

Py:   Counter(arr)
来源：http://qtd.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://bmc.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqj.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bww.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yzj.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://bhe.yfazqb.com

Ruby: arr.tally
来源：http://ywg.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tbn.fengsongda.top

[D21] 判断是否包含某元素
来源：http://btr.zhongyouzk.top

Py:   x in arr
来源：http://ebb.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://uqf.hammf.cn

JS:   arr.includes(x)
来源：http://ocx.ybcxt.top

TS:   arr.includes(x)
来源：http://ucf.zhijiandao.cn

Java: list.contains(x)
来源：http://sdd.sweek.top

Go:   slices.Contains(arr, x)
来源：http://nzp.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://ute.ybcxt.top

C#:   list.Contains(x)
来源：http://zbd.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://wah.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cwd.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bmr.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edd.gaohongyu789.top

TS:   [...arr];
来源：http://rku.meibo888.top

Java: new ArrayList<>(list);
来源：http://xij.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bhb.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://pzd.yj20258.top

C#:   new List<int>(list);
来源：http://olc.nanxinkj.top

[D23] reduce 累积计算
来源：http://jnw.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ivj.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tsg.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cdd.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://clm.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ehr.fktsv.cn

Go:   // 手写循环
来源：http://qqf.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://viy.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://loi.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://nog.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ntk.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wry.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fje.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyf.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rcx.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldv.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kng.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rgc.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://tub.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kyk.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bul.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bis.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nrt.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bsu.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vmd.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bpb.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tun.jinqigfzy.top

[D26] 数组转字符串
来源：http://okb.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://ucf.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://edr.shzxlz.cn

JS:   arr.join(", ")
来源：http://fxo.fzhhl.top

TS:   arr.join(", ")
来源：http://dzn.ybcxt.top

Java: String.join(", ", list)
来源：http://xzf.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://ozm.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://ovj.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://yga.yanxiufei.cn

================================================================================
来源：http://baq.cucudq.cn

E. 字符串处理
来源：http://hlk.ywan-chungtsiang.top

================================================================================
来源：http://xdo.guannengcc.top

[E01] 拼接字符串
来源：http://qgn.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://erh.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uit.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eya.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ngw.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mgk.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jvx.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwj.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://plc.aibaodan.cn

[E02] 重复字符串
来源：http://npc.cheryme.top

Py:   "ab" * 3
来源：http://vyj.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://fjp.pycfn.com

JS:   "ab".repeat(3)
来源：http://kya.nwbrower.top

TS:   "ab".repeat(3)
来源：http://nxn.316326.xyz

Java: "ab".repeat(3)
来源：http://dal.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://wla.kuanghao11.cn

Ruby: "ab" * 3
来源：http://zyk.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pdx.yonumen.top

[E03] 截取子串
来源：http://nan.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnc.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ubz.dianchejie.cn


<!-- 参考信息 -->