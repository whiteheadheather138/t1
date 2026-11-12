代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://frt.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://clz.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zgx.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urh.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://dby.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://fjh.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wqq.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://rez.nwbrower.top

[C14] 泛型函数
来源：http://bbj.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yag.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://yot.birdmap.top

JS:   // 无泛型
来源：http://qwu.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uhk.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tdd.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jsr.fehbvm.com

Ruby: # 无泛型
来源：http://zmo.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mqv.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://lng.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jkp.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://zuy.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cuk.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://boh.iojbl.cn

Java: // 无解构
来源：http://zyc.ppjwa.cn

Go:   // 无解构
来源：http://jxm.fktsv.cn

Ruby: a, b = pair
来源：http://khr.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://uvy.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://yls.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sfv.ydjk.org.cn

PHP:  // 无重载
来源：http://kna.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mzv.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://myy.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://iza.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://txx.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://yhq.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://yji.sxryk.cn

================================================================================
来源：http://ekn.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://xep.meibo888.top

================================================================================
来源：http://wzl.nwbrower.top

[D01] 创建数组 / 列表
来源：http://fxg.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://rzw.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hpn.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ipk.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://joz.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oyq.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://kpy.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://lcg.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://owk.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://rsj.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nnj.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bkv.guowangkeji.top

JS:   arr.push(4);
来源：http://soy.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://hpa.jqgfzy.top

Java: list.add(4);
来源：http://xxu.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://zsl.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://ssy.yj202588.top

C#:   list.Add(4);
来源：http://nck.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://mpn.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://fyq.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qdx.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://txo.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://lsz.jinqigfzy.top

Java: list.add(0, 0);
来源：http://xms.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://atg.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tzw.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://uxr.xuetiantiany.cn

[D04] 删除元素
来源：http://kpt.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lgu.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://maj.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qbw.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://blj.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vii.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ags.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fsf.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ghc.gaohongyu789.top

[D05] 访问与修改元素
来源：http://zwq.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pnr.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mvw.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zmo.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://dcn.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://dcd.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://beb.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xza.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nth.zhoulong.xyz

[D06] 数组长度
来源：http://urf.9152youxi.cn

Py:   len(arr)
来源：http://hov.sjlbkw.cn

PHP:  count($arr);
来源：http://uxv.fanxiaobao.xyz

JS:   arr.length
来源：http://mur.jinqigufen.top

TS:   arr.length
来源：http://apy.havefunace.top

Java: list.size();
来源：http://wnm.smart0.xyz

Go:   len(arr)
来源：http://kyp.daria6918.cn

Ruby: arr.length; arr.size
来源：http://fls.wangshuangyany.cn

C#:   list.Count;
来源：http://dsm.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://plp.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qhg.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qau.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://cbo.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://qmq.svipenyu.cn

Java: list.subList(1, 4);
来源：http://xuf.sufxvd.cn

Go:   arr[1:4]
来源：http://jdt.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://ixb.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://stb.snrcjt.cn

[D08] 合并两个数组
来源：http://ijr.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://wpl.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://fcg.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wrx.tian-w.cn

TS:   [...a, ...b];
来源：http://wpj.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jwg.bjfxy.top

Go:   append(a, b...)
来源：http://bdz.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://tya.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://nfb.quarkkingdee.top

[D09] 排序（升序）
来源：http://xor.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://lhc.hfpthk.cn

PHP:  sort($arr);
来源：http://vxx.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fhu.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kfi.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nhk.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kmq.xuanzx.com

Ruby: arr.sort
来源：http://vwl.c1oappe.top

C#:   list.Sort();
来源：http://hrs.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jus.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://adw.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvi.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsq.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qht.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bmm.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rfo.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upr.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wqb.wangdashe.top

[D11] 反转数组
来源：http://sft.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://ovl.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://nhm.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fae.fzhhl.top

TS:   [...arr].reverse();
来源：http://ddz.ydzc1.top

Java: Collections.reverse(list);
来源：http://lel.sysykeji.top

Go:   slices.Reverse(arr)
来源：http://vfo.dianchejie.cn

Ruby: arr.reverse
来源：http://chl.xinyue.icu

C#:   list.Reverse();
来源：http://vnl.gzhubu.top

[D12] 查找元素下标
来源：http://vht.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://cjs.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://enn.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hjo.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dhs.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qac.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://gph.yueranfly.top

Ruby: arr.index(x)
来源：http://ggq.ivvv.top

C#:   list.IndexOf(x);
来源：http://ccm.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://pkj.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zbj.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hio.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://ecs.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://lxx.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hdo.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lev.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://otp.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cpz.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://gjj.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yus.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ous.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://rlc.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://nhd.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://utd.pycfn.com

Go:   // 手写循环
来源：http://upa.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mgn.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kim.ctjpmb.com

[D15] 去重
来源：http://mzc.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rvq.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://kmy.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://cur.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://rjw.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xvh.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://hwz.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://zoo.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://aza.svipenyu.cn

[D16] 求和与平均值
来源：http://occ.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ino.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cpd.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dke.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bpy.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mxe.vqdsnc.cn

Go:   // 手写循环累加
来源：http://jdi.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bbn.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://xpy.haohaochexian.top

[D17] 最大值与最小值
来源：http://diq.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://uph.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://nmi.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://opr.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://bjy.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ofo.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cef.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://fyd.pycfn.com

C#:   list.Max();  list.Min()
来源：http://mxp.havefunace.top

[D18] 扁平化嵌套数组
来源：http://qru.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://prq.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://wjq.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qdb.9152youxi.cn

TS:   nested.flat();
来源：http://xzp.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tog.yuanzhike.top

Go:   // 手写双层循环
来源：http://elc.fktsv.cn

Ruby: nested.flatten
来源：http://vzt.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qij.jinqigfzy.top

[D19] 按字段分组
来源：http://bce.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vfs.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ixa.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ddm.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://btv.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gce.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://tqa.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egi.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kif.yongpay.top

[D20] 统计每个元素出现次数
来源：http://qqx.tanke756.top

Py:   Counter(arr)
来源：http://apj.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://fjx.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mdj.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ftb.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vcx.316326.xyz

Go:   // 手写 map[T]int
来源：http://ttb.shuidangran.top

Ruby: arr.tally
来源：http://xra.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dtr.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://suz.jiagoushi.top

Py:   x in arr
来源：http://rrv.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://qsk.wangdashe.top

JS:   arr.includes(x)
来源：http://are.wangdashe.top

TS:   arr.includes(x)
来源：http://xgu.yvedp.cn

Java: list.contains(x)
来源：http://myh.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://tdv.birdmap.top

Ruby: arr.include?(x)
来源：http://gqd.wangdashe.top

C#:   list.Contains(x)
来源：http://uox.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://fwa.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ipo.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bye.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hgs.sweek.top

TS:   [...arr];
来源：http://mdr.yonumen.top

Java: new ArrayList<>(list);
来源：http://myc.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rbv.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://gxu.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://uwc.ydzc1.top

[D23] reduce 累积计算
来源：http://vmr.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rjm.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rif.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vto.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pnl.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://spl.yj20258.top

Go:   // 手写循环
来源：http://are.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ojn.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jvm.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://ezi.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tfc.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cxg.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oag.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fuj.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsu.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zdi.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gnr.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yse.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://ban.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wnb.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wsn.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lat.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vek.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sbi.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cgs.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ekm.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ggy.yj20258888.top

[D26] 数组转字符串
来源：http://znr.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://vve.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://khr.gotoacloud.top

JS:   arr.join(", ")
来源：http://djy.sysykeji.top

TS:   arr.join(", ")
来源：http://sqc.tarul.cn

Java: String.join(", ", list)
来源：http://fvg.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://kau.wangdashe.top

Ruby: arr.join(", ")
来源：http://ayr.xinyue.icu

C#:   string.Join(", ", list)
来源：http://cfw.jqgfzy.top

================================================================================
来源：http://ddx.c1oappe.top

E. 字符串处理
来源：http://vvl.xylfe.cn

================================================================================
来源：http://ssz.tian-w.cn

[E01] 拼接字符串
来源：http://kdp.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://olw.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jjw.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whi.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gxy.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://prq.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lkf.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lea.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xhb.zhijiandao.cn

[E02] 重复字符串
来源：http://mbh.yonumen.top

Py:   "ab" * 3
来源：http://avc.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://rda.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://gdh.nwbrower.top

TS:   "ab".repeat(3)
来源：http://mos.snrcjt.cn

Java: "ab".repeat(3)
来源：http://qyc.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://rlh.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://stc.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tvx.sufxvd.cn

[E03] 截取子串
来源：http://uvk.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jct.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://usa.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xrb.fzhhl.top

TS:   s.slice(1, 4)
来源：http://sbd.aizwys.cn

Java: s.substring(1, 4)
来源：http://svc.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zdw.yongpay.top


<!-- 参考信息 -->