代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://rdl.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://kng.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wss.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://vgy.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tqa.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://odh.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://voq.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ktn.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://lov.zhengqikj.top

Go:   func add(a, b int) int
来源：http://wwz.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qhk.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://fae.wangdashe.top

[C14] 泛型函数
来源：http://vfn.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pts.tarul.cn

PHP:  // 无泛型
来源：http://wjx.ivvv.top

JS:   // 无泛型
来源：http://daq.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://esv.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cwl.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://csx.nanxuanxn.top

Ruby: # 无泛型
来源：http://cex.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ptn.tarul.cn

[C15] 解构 / 展开参数
来源：http://rml.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bev.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://gra.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bsa.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jwf.daxiang520.top

Java: // 无解构
来源：http://woh.sjlbkw.cn

Go:   // 无解构
来源：http://uvb.52xcode.cn

Ruby: a, b = pair
来源：http://ors.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://kvs.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://uwu.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://crv.nanxuanxn.top

PHP:  // 无重载
来源：http://vgf.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rdh.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://yri.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vds.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://sgk.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://cyh.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jli.hesvh.cn

================================================================================
来源：http://hlk.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://igd.316326.xyz

================================================================================
来源：http://bwx.jianghu66.top

[D01] 创建数组 / 列表
来源：http://zus.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://hpg.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ziz.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kth.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xlt.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ccn.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://hza.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://yno.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kcg.hcnkem.com

[D02] 追加元素到末尾
来源：http://odf.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xse.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rtg.tanke756.top

JS:   arr.push(4);
来源：http://fdb.xinyue.icu

TS:   arr.push(4);
来源：http://waw.jqgufenzy.top

Java: list.add(4);
来源：http://oqy.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://eva.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://cfj.yanxiufei.cn

C#:   list.Add(4);
来源：http://nex.yfazqb.com

[D03] 在指定位置插入元素
来源：http://rcw.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://scz.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uqb.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xhw.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://mge.vehdjk.com

Java: list.add(0, 0);
来源：http://hfu.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://hjm.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lii.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://tpu.jinqigufen.top

[D04] 删除元素
来源：http://uwg.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zky.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xvz.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pkv.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://xij.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aib.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsv.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sdl.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fcx.dashuyun.cn

[D05] 访问与修改元素
来源：http://yvx.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ruy.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vuq.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://usc.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://gey.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://bil.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://hgp.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cza.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gsa.tianlin.xyz

[D06] 数组长度
来源：http://yaq.chenjidiqi.icu

Py:   len(arr)
来源：http://dtz.zhixingplan.top

PHP:  count($arr);
来源：http://obz.bjfxy.top

JS:   arr.length
来源：http://qvn.hesvh.cn

TS:   arr.length
来源：http://nnq.tarul.cn

Java: list.size();
来源：http://ehv.ydjk.org.cn

Go:   len(arr)
来源：http://rjl.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://dxo.sjlbkw.cn

C#:   list.Count;
来源：http://oct.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ohk.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tor.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gkz.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://vax.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://wjl.yfazqb.com

Java: list.subList(1, 4);
来源：http://jbz.kuanghao11.cn

Go:   arr[1:4]
来源：http://tvt.tianlin.xyz

Ruby: arr[1, 3]
来源：http://nbs.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://ygp.0kj1m.cn

[D08] 合并两个数组
来源：http://skb.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://xrt.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://kzf.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://pqi.guowangkeji.top

TS:   [...a, ...b];
来源：http://qmt.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kph.yueranfly.top

Go:   append(a, b...)
来源：http://ycj.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://xcj.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://fys.pycfn.com

[D09] 排序（升序）
来源：http://vuj.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://xyz.andypj.xyz

PHP:  sort($arr);
来源：http://cjs.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://plh.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eif.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cxf.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nsh.xylfe.cn

Ruby: arr.sort
来源：http://ofh.yvedp.cn

C#:   list.Sort();
来源：http://ede.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://cbj.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yxq.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amo.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mgy.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzn.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lyg.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://syk.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xsw.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqm.zhixingplan.top

[D11] 反转数组
来源：http://pik.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://gko.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://ajv.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cnn.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://vjk.hfpthk.cn

Java: Collections.reverse(list);
来源：http://ldz.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://kpg.hammf.cn

Ruby: arr.reverse
来源：http://jsm.shzxlz.cn

C#:   list.Reverse();
来源：http://iug.redwolf501.top

[D12] 查找元素下标
来源：http://kac.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://wby.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mpp.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fiy.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zib.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xhj.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://vxv.cdnleiting.top

Ruby: arr.index(x)
来源：http://nqf.cashguo.top

C#:   list.IndexOf(x);
来源：http://zyp.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://kyd.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fvo.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xch.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://mzf.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://kwc.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cxv.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mph.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://iwf.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bgj.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://fvp.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bes.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mij.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://vfg.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://jdp.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aiq.hammf.cn

Go:   // 手写循环
来源：http://cay.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://gcb.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wmr.andypj.xyz

[D15] 去重
来源：http://vrm.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hpk.snrcjt.cn

PHP:  array_unique($arr);
来源：http://aie.yj20258888.top

JS:   [...new Set(arr)]
来源：http://mis.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://wmp.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uug.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://iax.sjlbkw.cn

Ruby: arr.uniq
来源：http://rks.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://xzj.52xcode.cn

[D16] 求和与平均值
来源：http://exx.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rbr.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://feq.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbj.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rvb.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cmh.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://iyi.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://guy.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://aop.gzhubu.top

[D17] 最大值与最小值
来源：http://dhu.yj202588.top

Py:   max(arr);  min(arr)
来源：http://ijg.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://utt.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nvt.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://ouz.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mch.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kkt.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://jsx.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://gwz.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://zjm.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xzu.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://uma.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lll.sweek.top

TS:   nested.flat();
来源：http://krw.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xls.pycfn.com

Go:   // 手写双层循环
来源：http://mwx.yongpay.top

Ruby: nested.flatten
来源：http://ney.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jdf.yangfankeji.com

[D19] 按字段分组
来源：http://ybs.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wvg.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bnd.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://twe.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dsc.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mjt.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://bih.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ehs.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://amq.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://yll.zhoulong.xyz

Py:   Counter(arr)
来源：http://amk.uphjek.com

PHP:  array_count_values($arr);
来源：http://lmh.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ppm.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://noz.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lpd.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://grh.xuanzx.com

Ruby: arr.tally
来源：http://nuq.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ffj.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://kja.tanke756.top

Py:   x in arr
来源：http://bgb.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://bwe.c1oappe.top

JS:   arr.includes(x)
来源：http://ebo.zhoulong.xyz

TS:   arr.includes(x)
来源：http://npg.tianlin.xyz

Java: list.contains(x)
来源：http://vji.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://hkc.sweek.top

Ruby: arr.include?(x)
来源：http://pwc.cheryme.top

C#:   list.Contains(x)
来源：http://jkj.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://hcb.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nnu.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uwp.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xyf.sxryk.cn

TS:   [...arr];
来源：http://rgf.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://rms.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://cuf.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://ent.xziqi.cn

C#:   new List<int>(list);
来源：http://wic.cqqwz.cn

[D23] reduce 累积计算
来源：http://ogs.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pyk.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pio.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vjl.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rpu.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gmn.cdnleiting.top

Go:   // 手写循环
来源：http://oga.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jro.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tah.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://vym.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nws.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sey.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ogn.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dhz.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://orb.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahn.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rbc.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uiv.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://kvi.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uda.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fmb.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qsi.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lkz.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://knt.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qey.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ksn.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oav.dianchejie.cn

[D26] 数组转字符串
来源：http://igr.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://eln.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://xos.dashuyun.cn

JS:   arr.join(", ")
来源：http://qja.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://zot.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://gae.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://cyk.316326.xyz

Ruby: arr.join(", ")
来源：http://wnv.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://qzp.hfpthk.cn

================================================================================
来源：http://aci.fzhhl.top

E. 字符串处理
来源：http://ffu.c1oappe.top

================================================================================
来源：http://jmw.cucudq.cn

[E01] 拼接字符串
来源：http://ulb.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wim.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rcg.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrv.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eqo.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rwp.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pcm.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qsg.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iue.jinqigfzy.top

[E02] 重复字符串
来源：http://ssd.daxiang520.top

Py:   "ab" * 3
来源：http://vhm.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://tqm.andypj.xyz

JS:   "ab".repeat(3)
来源：http://gbp.tarul.cn

TS:   "ab".repeat(3)
来源：http://jki.9152youxi.cn

Java: "ab".repeat(3)
来源：http://zkj.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://vrb.ybcxt.top

Ruby: "ab" * 3
来源：http://rdh.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpo.yueranfly.top

[E03] 截取子串
来源：http://ihe.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://czb.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yac.mhx1999.top


<!-- 参考信息 -->