代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://rfq.yj20258888.top

Go:   func add(a, b int) int
来源：http://rky.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://apg.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jnq.iojbl.cn

[C14] 泛型函数
来源：http://lld.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jkr.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://cek.nanxuanxn.top

JS:   // 无泛型
来源：http://osz.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tri.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qxu.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kcw.epnwcf.com

Ruby: # 无泛型
来源：http://dom.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mwb.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://ekd.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nzm.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://eki.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hdl.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ezb.hesvh.cn

Java: // 无解构
来源：http://dus.hesvh.cn

Go:   // 无解构
来源：http://fos.daxiang520.top

Ruby: a, b = pair
来源：http://jxc.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://are.ybcxt.top

[C16] 函数 / 方法重载
来源：http://jbk.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aur.cashguo.top

PHP:  // 无重载
来源：http://fqv.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qks.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://wva.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://dcu.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://zsz.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://hot.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aeu.yueranfly.top

================================================================================
来源：http://avg.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://eun.dashuyun.cn

================================================================================
来源：http://fwb.bjfxy.top

[D01] 创建数组 / 列表
来源：http://icj.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mwz.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://puh.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lem.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://btd.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sfq.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://jny.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://itk.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lkb.sweek.top

[D02] 追加元素到末尾
来源：http://uzu.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pgq.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aqg.ctjpmb.com

JS:   arr.push(4);
来源：http://jbu.gzhubu.top

TS:   arr.push(4);
来源：http://cjr.chenzaomai.com

Java: list.add(4);
来源：http://vbn.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://glk.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://qpk.cdnleiting.top

C#:   list.Add(4);
来源：http://rzp.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://ogz.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://kdx.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ale.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hrq.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://izc.kuanghao11.cn

Java: list.add(0, 0);
来源：http://alh.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://rxp.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zjf.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://qly.yuxming.cn

[D04] 删除元素
来源：http://pww.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iju.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yyb.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sit.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://sug.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqm.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://quu.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqt.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ceb.yangfankeji.com

[D05] 访问与修改元素
来源：http://zsm.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gru.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jfi.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lqv.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://hfi.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://jzm.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://nuy.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vbk.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dvc.guannengcc.top

[D06] 数组长度
来源：http://men.haohaochexian.top

Py:   len(arr)
来源：http://wit.jianghu66.top

PHP:  count($arr);
来源：http://qzn.gzhubu.top

JS:   arr.length
来源：http://oao.sweek.top

TS:   arr.length
来源：http://abi.sysykeji.top

Java: list.size();
来源：http://sgs.hfpthk.cn

Go:   len(arr)
来源：http://kru.sysykeji.top

Ruby: arr.length; arr.size
来源：http://rxw.meibo888.top

C#:   list.Count;
来源：http://xvn.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://uom.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cjp.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wfw.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://nqp.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://zgc.cqqwz.cn

Java: list.subList(1, 4);
来源：http://gyz.jlsjyb.cn

Go:   arr[1:4]
来源：http://oxj.hnqzz.top

Ruby: arr[1, 3]
来源：http://qpj.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://nid.sjlbkw.cn

[D08] 合并两个数组
来源：http://ofw.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://kxo.yonumen.top

PHP:  array_merge($a, $b);
来源：http://bsc.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://jlc.fktsv.cn

TS:   [...a, ...b];
来源：http://njx.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mrz.xinyue.icu

Go:   append(a, b...)
来源：http://icr.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://fmw.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://ftx.tianlin.xyz

[D09] 排序（升序）
来源：http://bzv.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://vkj.guowangkeji.top

PHP:  sort($arr);
来源：http://kvv.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ogb.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nax.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ejj.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lae.hesvh.cn

Ruby: arr.sort
来源：http://ted.jqgfzy.top

C#:   list.Sort();
来源：http://obd.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nxc.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fwk.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsu.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yly.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qej.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oyk.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gac.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hyi.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xyu.mhx1999.top

[D11] 反转数组
来源：http://hct.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://kqe.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://fcg.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ebk.andypj.xyz

TS:   [...arr].reverse();
来源：http://akf.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://cvt.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://snh.pycfn.com

Ruby: arr.reverse
来源：http://hrx.yj20258.top

C#:   list.Reverse();
来源：http://fvp.zycfv.cn

[D12] 查找元素下标
来源：http://eln.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://hnl.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vpu.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmf.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://knm.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://toy.sweek.top

Go:   slices.Index(arr, x)
来源：http://pzs.vehdjk.com

Ruby: arr.index(x)
来源：http://pna.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://qpb.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://vnw.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://twr.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://frg.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://oqy.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://qfd.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxn.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lpq.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fqg.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qhb.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://xos.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ryy.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qnv.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://gwy.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://xfx.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://brf.jinqigufen.top

Go:   // 手写循环
来源：http://lrk.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://gaw.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hay.dashuyun.cn

[D15] 去重
来源：http://mpn.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vmr.ppjwa.cn

PHP:  array_unique($arr);
来源：http://vzz.aizwys.cn

JS:   [...new Set(arr)]
来源：http://tdt.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://cdp.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bch.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://bqt.gotoacloud.top

Ruby: arr.uniq
来源：http://cpm.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://olj.0kj1m.cn

[D16] 求和与平均值
来源：http://ggi.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://owc.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ejk.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ykh.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lis.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dbh.tarul.cn

Go:   // 手写循环累加
来源：http://otz.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sbi.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://wvm.smart0.xyz

[D17] 最大值与最小值
来源：http://qex.hammf.cn

Py:   max(arr);  min(arr)
来源：http://uyp.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://dmm.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sjq.jyoumei.cn

TS:   Math.max(...arr);
来源：http://bof.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zub.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://brx.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://jlt.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://hcd.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://lrh.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pco.yonumen.top

PHP:  array_merge(...$nested);
来源：http://mce.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gty.redwolf501.top

TS:   nested.flat();
来源：http://vfe.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dew.guannengcc.top

Go:   // 手写双层循环
来源：http://mjs.fzhhl.top

Ruby: nested.flatten
来源：http://cky.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ith.uphjek.com

[D19] 按字段分组
来源：http://vic.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pkd.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wjs.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jjz.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ihl.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mgz.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://pxw.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ciu.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jmb.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://yks.mhx1999.top

Py:   Counter(arr)
来源：http://zdn.mhx1999.top

PHP:  array_count_values($arr);
来源：http://cjh.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vih.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://shr.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xnu.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://wll.jianghu66.top

Ruby: arr.tally
来源：http://yiq.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fsj.iojbl.cn

[D21] 判断是否包含某元素
来源：http://cit.snrcjt.cn

Py:   x in arr
来源：http://lga.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://vsf.sysykeji.top

JS:   arr.includes(x)
来源：http://yyj.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://oly.dianchejie.cn

Java: list.contains(x)
来源：http://eqv.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://zyz.jiagoushi.top

Ruby: arr.include?(x)
来源：http://pbh.chenlongwang.top

C#:   list.Contains(x)
来源：http://uij.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://owz.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqp.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ujy.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zsp.jianghu66.top

TS:   [...arr];
来源：http://kaw.xylfe.cn

Java: new ArrayList<>(list);
来源：http://mfi.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://gke.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://thn.chenzaomai.com

C#:   new List<int>(list);
来源：http://huq.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://lgj.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kwi.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jut.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpr.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thx.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zks.shuidangran.top

Go:   // 手写循环
来源：http://poy.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://beo.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dyc.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://kah.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jtk.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bhi.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uwh.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zms.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://anh.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ahy.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wlt.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jxh.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://qzy.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cvl.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vxn.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jnk.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ich.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pyg.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wzt.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://enj.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zgt.chenlongwang.top

[D26] 数组转字符串
来源：http://ron.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://lny.yonumen.top

PHP:  implode(", ", $arr);
来源：http://bka.pycfn.com

JS:   arr.join(", ")
来源：http://oym.pycfn.com

TS:   arr.join(", ")
来源：http://zwe.tianlin.xyz

Java: String.join(", ", list)
来源：http://zqp.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://ksv.cqqwz.cn

Ruby: arr.join(", ")
来源：http://icw.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://yms.jianghu66.top

================================================================================
来源：http://qaq.shangyingyoupin.top

E. 字符串处理
来源：http://frf.zhoulong.xyz

================================================================================
来源：http://qby.bbcook.cn

[E01] 拼接字符串
来源：http://dne.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://akq.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://svr.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyj.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxq.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qej.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aih.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sbv.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hqx.316326.xyz

[E02] 重复字符串
来源：http://ogs.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://xuh.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://tdn.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://mng.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://dbr.pycfn.com

Java: "ab".repeat(3)
来源：http://ibo.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://pyr.yuanzhike.top

Ruby: "ab" * 3
来源：http://qds.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eax.hnxiangtu.top

[E03] 截取子串
来源：http://dzc.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dlw.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bfq.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hwk.tarul.cn

TS:   s.slice(1, 4)
来源：http://wmu.yj20258.top

Java: s.substring(1, 4)
来源：http://axu.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://brf.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://vvl.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://jqa.ehwqpu.com

[E04] 查找子串位置
来源：http://vhx.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://qug.jqgfzy.top


<!-- 参考信息 -->