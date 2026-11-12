代发 wailian999

[C14] 泛型函数
来源：http://skw.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ram.hcnkem.com

PHP:  // 无泛型
来源：http://fau.guowangkeji.top

JS:   // 无泛型
来源：http://pun.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ztz.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dnk.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bfn.kuanghao11.cn

Ruby: # 无泛型
来源：http://lun.nanxuanxn.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nlf.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://vry.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xdb.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://zke.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wsv.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fyl.jqgfzy.top

Java: // 无解构
来源：http://wgh.gzhubu.top

Go:   // 无解构
来源：http://ifi.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://sjv.birdmap.top

C#:   var (a, b) = pair;
来源：http://lwx.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://ljc.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxc.zdbjq.cn

PHP:  // 无重载
来源：http://thz.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ztg.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://qyw.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rfp.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://tfk.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://hjq.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://npx.aibaodan.cn

================================================================================
来源：http://glv.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://vzb.chenlongwang.top

================================================================================
来源：http://qyi.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://jdq.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://vcc.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xib.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eeg.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wed.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzz.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://lsv.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://yzu.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uza.xuanzx.com

[D02] 追加元素到末尾
来源：http://gqj.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qll.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vsi.tian-w.cn

JS:   arr.push(4);
来源：http://sat.aibaodan.cn

TS:   arr.push(4);
来源：http://hyo.birdmap.top

Java: list.add(4);
来源：http://gzn.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://dwp.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://jnd.chenjidiqi.icu

C#:   list.Add(4);
来源：http://hlq.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://bco.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://mya.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eup.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vqs.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://huw.svipenyu.cn

Java: list.add(0, 0);
来源：http://bqp.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://qdl.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xkw.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://avb.yanxiufei.cn

[D04] 删除元素
来源：http://odx.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqq.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pxc.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hbc.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://hgu.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xtt.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blb.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kom.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yht.mhx1999.top

[D05] 访问与修改元素
来源：http://duk.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kui.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://byj.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zpg.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://ogm.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://frr.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://yuy.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dhh.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tig.shanyushiyangkeji.top

[D06] 数组长度
来源：http://hda.hesvh.cn

Py:   len(arr)
来源：http://obp.zhongyouzk.top

PHP:  count($arr);
来源：http://eme.fktsv.cn

JS:   arr.length
来源：http://fra.jinqigfzy.top

TS:   arr.length
来源：http://xsr.yvedp.cn

Java: list.size();
来源：http://hpy.daria6918.cn

Go:   len(arr)
来源：http://ngn.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://yvq.sufxvd.cn

C#:   list.Count;
来源：http://ayf.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://tcs.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wpw.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://xpa.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://iuj.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://xho.xinyue.icu

Java: list.subList(1, 4);
来源：http://hhr.yj20258888.top

Go:   arr[1:4]
来源：http://xau.sxryk.cn

Ruby: arr[1, 3]
来源：http://mdi.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://oqe.wangdashe.top

[D08] 合并两个数组
来源：http://wzv.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://gnt.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://vnc.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kra.c1oappe.top

TS:   [...a, ...b];
来源：http://lue.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://itd.nwbrower.top

Go:   append(a, b...)
来源：http://diu.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://hzc.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://eeo.feifeiyinyue.top

[D09] 排序（升序）
来源：http://qva.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://ptm.ctjpmb.com

PHP:  sort($arr);
来源：http://omy.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gya.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cex.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ibg.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qwg.kuanghao11.cn

Ruby: arr.sort
来源：http://kcb.redwolf501.top

C#:   list.Sort();
来源：http://czf.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nuy.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mtt.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yka.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eva.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zte.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pmg.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yqo.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://evm.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kpb.dianchejie.cn

[D11] 反转数组
来源：http://xwd.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://rcp.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://ugq.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oce.tianlin.xyz

TS:   [...arr].reverse();
来源：http://fhd.guowangkeji.top

Java: Collections.reverse(list);
来源：http://dda.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://udu.pengpengdd.cyou

Ruby: arr.reverse
来源：http://rzg.daria6918.cn

C#:   list.Reverse();
来源：http://oov.sweek.top

[D12] 查找元素下标
来源：http://ipb.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://rda.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sqs.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yhd.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqu.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bml.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://sft.snrcjt.cn

Ruby: arr.index(x)
来源：http://qeo.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://oet.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://tun.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pjf.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://alh.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://fzx.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://udg.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ysh.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wcr.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://yqf.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dns.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://sdr.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sfa.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mrw.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://mcn.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://gpe.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://lab.haohaochexian.top

Go:   // 手写循环
来源：http://vnr.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://tlw.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zaj.316326.xyz

[D15] 去重
来源：http://brm.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://thk.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://ola.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://xma.cucudq.cn

TS:   [...new Set(arr)]
来源：http://faj.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jwy.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://jzs.sufxvd.cn

Ruby: arr.uniq
来源：http://ila.nanxuanxn.top

C#:   list.Distinct().ToList()
来源：http://dho.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://pgy.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cke.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://svu.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpb.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wel.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jum.yongpay.top

Go:   // 手写循环累加
来源：http://agg.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ieo.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://rmc.sxryk.cn

[D17] 最大值与最小值
来源：http://uqa.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://lla.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://kid.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vvg.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://xur.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qim.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://whv.havefunace.top

Ruby: arr.max;  arr.min
来源：http://ckv.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://kba.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://lqz.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iye.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://whm.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://okg.guannengcc.top

TS:   nested.flat();
来源：http://sez.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fws.ctjpmb.com

Go:   // 手写双层循环
来源：http://sdd.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://mhy.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nmo.chenzaomai.com

[D19] 按字段分组
来源：http://jmu.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vta.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dwy.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpu.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwn.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vpk.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://tcn.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://dar.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://plq.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://ztk.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://hkl.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://die.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atu.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iry.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hgf.sxryk.cn

Go:   // 手写 map[T]int
来源：http://ufv.dashuyun.cn

Ruby: arr.tally
来源：http://hed.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tdq.fzhhl.top

[D21] 判断是否包含某元素
来源：http://bew.tarul.cn

Py:   x in arr
来源：http://ped.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://lng.52xcode.cn

JS:   arr.includes(x)
来源：http://vsa.zhongyouzk.top

TS:   arr.includes(x)
来源：http://kev.nanxuanxn.top

Java: list.contains(x)
来源：http://lrh.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://txw.iojbl.cn

Ruby: arr.include?(x)
来源：http://drp.hywenlv.cn

C#:   list.Contains(x)
来源：http://yxi.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://ddu.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yyy.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ymh.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://htz.hongshengwenyu.top

TS:   [...arr];
来源：http://asm.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://zee.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bla.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://zhp.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://cyr.sweek.top

[D23] reduce 累积计算
来源：http://zql.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hor.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hdi.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbu.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqc.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kee.9152youxi.cn

Go:   // 手写循环
来源：http://ipe.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zxu.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://auo.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://wmb.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://adc.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xme.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kfi.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nrb.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qqx.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ese.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kwg.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejt.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://ing.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gcy.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ose.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cdh.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wdp.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fxp.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lal.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uln.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wom.vqdsnc.cn

[D26] 数组转字符串
来源：http://gab.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://wse.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://tkb.hnxiangtu.top

JS:   arr.join(", ")
来源：http://ndt.daxiang520.top

TS:   arr.join(", ")
来源：http://uya.svipenyu.cn

Java: String.join(", ", list)
来源：http://cvr.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://vln.hywenlv.cn

Ruby: arr.join(", ")
来源：http://mtf.bbcook.cn

C#:   string.Join(", ", list)
来源：http://bpp.shanyushiyangkeji.top

================================================================================
来源：http://aog.tianlin.xyz

E. 字符串处理
来源：http://oza.yj202588.top

================================================================================
来源：http://skb.haohaochexian.top

[E01] 拼接字符串
来源：http://iyp.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kwg.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://evo.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygk.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxv.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jdz.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tap.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gqe.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ila.52xcode.cn

[E02] 重复字符串
来源：http://qpf.ppjwa.cn

Py:   "ab" * 3
来源：http://pip.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://fii.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://fkn.pycfn.com

TS:   "ab".repeat(3)
来源：http://fue.ctjpmb.com

Java: "ab".repeat(3)
来源：http://nls.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://ygl.xylfe.cn

Ruby: "ab" * 3
来源：http://gfm.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gnm.ivvv.top

[E03] 截取子串
来源：http://psu.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oum.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nxc.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bco.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://kba.yuxming.cn

Java: s.substring(1, 4)
来源：http://sdt.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ddj.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://fzu.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://mpp.birdmap.top

[E04] 查找子串位置
来源：http://xqz.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://ece.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://eby.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fbk.yvedp.cn

TS:   s.indexOf("x")
来源：http://urp.jqgfzy.top

Java: s.indexOf("x")
来源：http://fgk.andypj.xyz


<!-- 参考信息 -->