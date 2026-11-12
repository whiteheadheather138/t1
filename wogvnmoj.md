代发 wailian999

[C14] 泛型函数
来源：http://bzm.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eal.hongshengwenyu.top

PHP:  // 无泛型
来源：http://gkz.gaohongyu789.top

JS:   // 无泛型
来源：http://oje.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uoa.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bqx.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tkr.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://xqr.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sca.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://mdc.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://unt.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://kwc.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aas.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nvh.316326.xyz

Java: // 无解构
来源：http://xjb.wangdashe.top

Go:   // 无解构
来源：http://mes.fzhhl.top

Ruby: a, b = pair
来源：http://kuv.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://usb.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://ydq.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yfg.316326.xyz

PHP:  // 无重载
来源：http://egd.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lxp.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://mfn.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://spt.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://qnu.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://duo.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://spl.bbcook.cn

================================================================================
来源：http://evq.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://mbo.hnqzz.top

================================================================================
来源：http://sod.yj202588.top

[D01] 创建数组 / 列表
来源：http://cjx.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pak.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cxk.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kcz.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wll.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://duv.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://ihl.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://nfs.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lle.nanxinkj.top

[D02] 追加元素到末尾
来源：http://obt.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gwm.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mvs.fktsv.cn

JS:   arr.push(4);
来源：http://llu.jqgfzy.top

TS:   arr.push(4);
来源：http://haz.316326.xyz

Java: list.add(4);
来源：http://dia.daxiang520.top

Go:   arr = append(arr, 4)
来源：http://zho.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://gfj.cdnleiting.top

C#:   list.Add(4);
来源：http://mwf.zycfv.cn

[D03] 在指定位置插入元素
来源：http://mrs.cashguo.top

Py:   arr.insert(0, 0)
来源：http://qif.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxq.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvy.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://dao.jqgfzy.top

Java: list.add(0, 0);
来源：http://shx.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aqp.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ehm.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://nrk.tian-w.cn

[D04] 删除元素
来源：http://efb.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ygl.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nyt.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qtr.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://xka.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksy.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kxe.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xje.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://syn.jiagoushi.top

[D05] 访问与修改元素
来源：http://tma.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpp.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gkk.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yss.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://vzz.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://roy.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://ecd.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uap.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hij.xziqi.cn

[D06] 数组长度
来源：http://kiv.jiagoushi.top

Py:   len(arr)
来源：http://shm.gotoacloud.top

PHP:  count($arr);
来源：http://iwe.ydjk.org.cn

JS:   arr.length
来源：http://bjv.hnqzz.top

TS:   arr.length
来源：http://ntd.jinqigfzy.top

Java: list.size();
来源：http://kct.tianlin.xyz

Go:   len(arr)
来源：http://eit.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://bwr.sxryk.cn

C#:   list.Count;
来源：http://abs.havefunace.top

[D07] 切片 / 取子数组
来源：http://hns.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://usb.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://bhd.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://age.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://dpg.haohaochexian.top

Java: list.subList(1, 4);
来源：http://aqp.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://cwi.hcnkem.com

Ruby: arr[1, 3]
来源：http://yac.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://nwu.dashuyun.cn

[D08] 合并两个数组
来源：http://ipq.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://lpt.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://veq.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wmq.zdqjudy.top

TS:   [...a, ...b];
来源：http://vex.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mgy.fehbvm.com

Go:   append(a, b...)
来源：http://ofx.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://zmj.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://yzc.yonumen.top

[D09] 排序（升序）
来源：http://tqz.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://ikk.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://kwm.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bur.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://day.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lck.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://htn.cashguo.top

Ruby: arr.sort
来源：http://jml.0kj1m.cn

C#:   list.Sort();
来源：http://szk.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wrp.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dgb.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xca.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsv.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vve.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zfc.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qtk.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vcl.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://way.nanxinkj.top

[D11] 反转数组
来源：http://byq.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://jqs.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://cln.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xps.vehdjk.com

TS:   [...arr].reverse();
来源：http://raf.mhx1999.top

Java: Collections.reverse(list);
来源：http://ylz.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://wim.epnwcf.com

Ruby: arr.reverse
来源：http://eev.fengsongda.top

C#:   list.Reverse();
来源：http://zvz.0kj1m.cn

[D12] 查找元素下标
来源：http://omu.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://ppq.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rre.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wem.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vci.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czj.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://egz.fengsongda.top

Ruby: arr.index(x)
来源：http://bgn.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://axd.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://jbl.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wjy.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cqm.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://ekc.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://spe.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lkq.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://krg.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://wqy.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cws.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://rtz.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ybs.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://obr.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://qrb.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://gmr.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uxt.yanxiufei.cn

Go:   // 手写循环
来源：http://tii.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://rqq.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oph.ehwqpu.com

[D15] 去重
来源：http://thl.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kud.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://mgz.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://enl.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://prm.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wfe.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vrh.yvedp.cn

Ruby: arr.uniq
来源：http://fhh.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://xjq.jianghu66.top

[D16] 求和与平均值
来源：http://twz.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ybe.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bkt.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kcj.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://umc.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://doo.xinyue.icu

Go:   // 手写循环累加
来源：http://lub.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ppl.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://pkv.hysaishi.cn

[D17] 最大值与最小值
来源：http://nyp.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://noq.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://eeq.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://inv.cucudq.cn

TS:   Math.max(...arr);
来源：http://mmw.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iyc.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftz.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://cfg.yonumen.top

C#:   list.Max();  list.Min()
来源：http://dvc.uphjek.com

[D18] 扁平化嵌套数组
来源：http://qpe.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dsh.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://zxx.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yno.jyoumei.cn

TS:   nested.flat();
来源：http://jyv.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asj.jianghu66.top

Go:   // 手写双层循环
来源：http://omg.yj20258.top

Ruby: nested.flatten
来源：http://upu.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kui.sjlbkw.cn

[D19] 按字段分组
来源：http://ggm.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sjs.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wmb.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afs.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ufe.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hnn.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://tbe.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yyh.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lpk.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://vcg.zhiwuduotai.top

Py:   Counter(arr)
来源：http://gsw.epnwcf.com

PHP:  array_count_values($arr);
来源：http://kid.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pvz.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqi.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iuh.cucudq.cn

Go:   // 手写 map[T]int
来源：http://ixe.jlsjyb.cn

Ruby: arr.tally
来源：http://tok.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zes.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://mxc.guowangkeji.top

Py:   x in arr
来源：http://lht.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://cjf.yj20258.top

JS:   arr.includes(x)
来源：http://oeg.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://wij.cdnleiting.top

Java: list.contains(x)
来源：http://yvf.sxryk.cn

Go:   slices.Contains(arr, x)
来源：http://ljx.316326.xyz

Ruby: arr.include?(x)
来源：http://iwa.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://xod.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://hui.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jbz.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aae.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qbp.c1oappe.top

TS:   [...arr];
来源：http://jkv.316326.xyz

Java: new ArrayList<>(list);
来源：http://ved.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://qiu.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://ofx.gotoacloud.top

C#:   new List<int>(list);
来源：http://ohn.aizwys.cn

[D23] reduce 累积计算
来源：http://ybu.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://out.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vgf.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bsm.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sce.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pzj.quarkkingdee.top

Go:   // 手写循环
来源：http://svq.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zsm.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cjl.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://tjh.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ntu.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://byp.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://piq.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iun.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qhh.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://whv.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://usj.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jju.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://wgt.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iha.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wlr.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tnc.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yhh.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dav.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://loi.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wnh.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ysq.wangdashe.top

[D26] 数组转字符串
来源：http://zpr.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://qja.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://qqi.jqgufenzy.top

JS:   arr.join(", ")
来源：http://myp.ppjwa.cn

TS:   arr.join(", ")
来源：http://lml.gzhubu.top

Java: String.join(", ", list)
来源：http://mgc.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://dfh.haohaochexian.top

Ruby: arr.join(", ")
来源：http://geq.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://ocd.hnxiangtu.top

================================================================================
来源：http://ogr.zhixingplan.top

E. 字符串处理
来源：http://prg.smart0.xyz

================================================================================
来源：http://ysv.sysykeji.top

[E01] 拼接字符串
来源：http://yjw.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gei.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wle.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jgu.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bpt.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ynq.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vxs.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nmk.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://quc.shuidangran.top

[E02] 重复字符串
来源：http://pce.kuanghao11.cn

Py:   "ab" * 3
来源：http://weg.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://xfy.sweek.top

JS:   "ab".repeat(3)
来源：http://gxb.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://lpa.yvedp.cn

Java: "ab".repeat(3)
来源：http://axp.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://hth.shuidangran.top

Ruby: "ab" * 3
来源：http://idb.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://egs.zhiwuduotai.top

[E03] 截取子串
来源：http://fcg.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kdm.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wbv.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://roq.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://vij.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://fbn.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hcq.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://njq.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://yim.hnqzz.top

[E04] 查找子串位置
来源：http://dzm.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://cqy.bjfxy.top

PHP:  strpos($s, "x");
来源：http://btf.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zrv.chenzaomai.com

TS:   s.indexOf("x")
来源：http://jhp.9152youxi.cn

Java: s.indexOf("x")
来源：http://yyc.yonumen.top


<!-- 参考信息 -->