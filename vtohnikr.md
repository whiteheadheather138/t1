代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://jjm.shzxlz.cn

Go:   func add(a, b int) int
来源：http://nvi.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wdd.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpq.aizwys.cn

[C14] 泛型函数
来源：http://cqj.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cck.hongshengwenyu.top

PHP:  // 无泛型
来源：http://xou.yueranfly.top

JS:   // 无泛型
来源：http://tle.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://afr.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqv.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rnn.316326.xyz

Ruby: # 无泛型
来源：http://alh.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qkc.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://hws.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xzo.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://xmm.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pny.zhiwuduotai.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dum.tanke756.top

Java: // 无解构
来源：http://ewx.gaohongyu789.top

Go:   // 无解构
来源：http://klh.shzxlz.cn

Ruby: a, b = pair
来源：http://isk.smart0.xyz

C#:   var (a, b) = pair;
来源：http://vfp.havefunace.top

[C16] 函数 / 方法重载
来源：http://rld.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iwn.fzhhl.top

PHP:  // 无重载
来源：http://bul.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ezr.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://uca.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dso.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://wla.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://yiw.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nyt.quarkkingdee.top

================================================================================
来源：http://hfd.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://mkj.sufxvd.cn

================================================================================
来源：http://qcs.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://kkj.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqo.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eyt.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vtl.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://srt.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dgf.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://lea.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://res.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ebm.yj202588.top

[D02] 追加元素到末尾
来源：http://ypu.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lgb.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ynd.gaohongyu789.top

JS:   arr.push(4);
来源：http://eno.birdmap.top

TS:   arr.push(4);
来源：http://ild.tian-w.cn

Java: list.add(4);
来源：http://ahr.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://wwh.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://imf.nanxinkj.top

C#:   list.Add(4);
来源：http://syp.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://fly.tarul.cn

Py:   arr.insert(0, 0)
来源：http://wrn.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://det.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fnf.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://avb.jqgfzy.top

Java: list.add(0, 0);
来源：http://ssh.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://thb.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdw.tanke756.top

C#:   list.Insert(0, 0);
来源：http://yej.52xcode.cn

[D04] 删除元素
来源：http://kkr.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nyp.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yvy.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mij.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://xnf.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dsp.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://huk.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bkr.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dpj.sxryk.cn

[D05] 访问与修改元素
来源：http://pna.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxg.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://udl.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xmc.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://yyq.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://hyg.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://erw.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://frb.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://top.jinqigfzy.top

[D06] 数组长度
来源：http://uoa.xylfe.cn

Py:   len(arr)
来源：http://xan.jinghuilouyu.cn

PHP:  count($arr);
来源：http://yvx.zycfv.cn

JS:   arr.length
来源：http://bgk.zhengqikj.top

TS:   arr.length
来源：http://hch.sysykeji.top

Java: list.size();
来源：http://knu.wangdashe.top

Go:   len(arr)
来源：http://ctl.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://nnn.nwbrower.top

C#:   list.Count;
来源：http://ddl.hcnkem.com

[D07] 切片 / 取子数组
来源：http://rys.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ptp.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oid.birdmap.top

JS:   arr.slice(1, 4);
来源：http://ruy.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://luc.epnwcf.com

Java: list.subList(1, 4);
来源：http://zhv.sufxvd.cn

Go:   arr[1:4]
来源：http://zfb.316326.xyz

Ruby: arr[1, 3]
来源：http://iqx.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://jmo.snrcjt.cn

[D08] 合并两个数组
来源：http://fbo.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://iij.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://vat.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qmw.zycfv.cn

TS:   [...a, ...b];
来源：http://twc.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vqa.fzhhl.top

Go:   append(a, b...)
来源：http://eff.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://dxf.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://tnr.sweek.top

[D09] 排序（升序）
来源：http://nhz.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ezk.birdmap.top

PHP:  sort($arr);
来源：http://tuz.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yja.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zmg.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xhs.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dzl.fzhhl.top

Ruby: arr.sort
来源：http://fbk.gaohongyu789.top

C#:   list.Sort();
来源：http://win.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kwp.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xfc.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://grf.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vxp.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgl.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kwy.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://idn.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ghb.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://khj.zycfv.cn

[D11] 反转数组
来源：http://mor.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://ouj.smart0.xyz

PHP:  array_reverse($arr);
来源：http://knl.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vsj.fzhhl.top

TS:   [...arr].reverse();
来源：http://iqi.aibaodan.cn

Java: Collections.reverse(list);
来源：http://xut.yj20258.top

Go:   slices.Reverse(arr)
来源：http://hfu.sufxvd.cn

Ruby: arr.reverse
来源：http://pui.guowangkeji.top

C#:   list.Reverse();
来源：http://kcn.havefunace.top

[D12] 查找元素下标
来源：http://usg.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://ice.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://syw.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ias.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjm.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://edp.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://zre.uphjek.com

Ruby: arr.index(x)
来源：http://nfc.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://pge.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://yxg.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rpl.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://irv.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://nnr.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://htl.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gfy.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://umn.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gxj.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://xxt.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://fzu.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rib.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jwu.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://rnn.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://rdp.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://znw.meibo888.top

Go:   // 手写循环
来源：http://hmg.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oel.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rgv.aizwys.cn

[D15] 去重
来源：http://zuf.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://efc.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://omb.birdmap.top

JS:   [...new Set(arr)]
来源：http://oat.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://foq.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://urq.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://roa.jinqigufen.top

Ruby: arr.uniq
来源：http://otp.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://kpv.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://hvm.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vle.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xga.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sot.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfy.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nvs.yuanzhike.top

Go:   // 手写循环累加
来源：http://gij.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mde.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://eof.aibaodan.cn

[D17] 最大值与最小值
来源：http://cnk.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://qqj.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://ctf.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://njy.redwolf501.top

TS:   Math.max(...arr);
来源：http://eiu.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gwn.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rjk.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://lmh.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://hyb.tanke756.top

[D18] 扁平化嵌套数组
来源：http://bdx.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xjz.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://tws.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wkq.cashguo.top

TS:   nested.flat();
来源：http://ael.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yru.cqqwz.cn

Go:   // 手写双层循环
来源：http://fzr.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://xbu.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://whm.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://mtl.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hgh.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ubf.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://txj.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qlb.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vdm.uphjek.com

Go:   // 手写 map[string][]T
来源：http://lwl.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://paa.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xsg.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://sks.birdmap.top

Py:   Counter(arr)
来源：http://ked.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://xnb.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fco.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wmk.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tln.fehbvm.com

Go:   // 手写 map[T]int
来源：http://zuz.ehwqpu.com

Ruby: arr.tally
来源：http://eqw.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kbm.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://gfz.gzhubu.top

Py:   x in arr
来源：http://ncu.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://lua.hnqzz.top

JS:   arr.includes(x)
来源：http://ira.gotoacloud.top

TS:   arr.includes(x)
来源：http://jww.hesvh.cn

Java: list.contains(x)
来源：http://tle.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://evb.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://vpp.fzhhl.top

C#:   list.Contains(x)
来源：http://npj.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://uja.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://udk.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cmo.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vwl.guannengcc.top

TS:   [...arr];
来源：http://kjh.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://uui.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://hnk.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://ecb.wangdashe.top

C#:   new List<int>(list);
来源：http://xil.chenlongwang.top

[D23] reduce 累积计算
来源：http://qqr.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqr.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gtm.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ifv.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozm.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rff.vqdsnc.cn

Go:   // 手写循环
来源：http://obj.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ymr.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cju.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://mkv.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qpn.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fqi.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rjf.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ijf.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://obs.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dmi.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://raa.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xak.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://kmi.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lyy.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hcd.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hhq.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://woh.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wia.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://shn.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cxp.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://imu.jiagoushi.top

[D26] 数组转字符串
来源：http://pzo.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://uhz.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://ccf.yonumen.top

JS:   arr.join(", ")
来源：http://foq.xziqi.cn

TS:   arr.join(", ")
来源：http://ysd.jlsjyb.cn

Java: String.join(", ", list)
来源：http://hto.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://dmk.jiagoushi.top

Ruby: arr.join(", ")
来源：http://fur.fengsongda.top

C#:   string.Join(", ", list)
来源：http://zxu.meibo888.top

================================================================================
来源：http://tao.shanyushiyangtech.top

E. 字符串处理
来源：http://fgu.shanyushiyangkeji.top

================================================================================
来源：http://dop.havefunace.top

[E01] 拼接字符串
来源：http://oqp.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oog.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tyr.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://utw.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pjo.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rge.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pqq.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://upn.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rng.meibo888.top

[E02] 重复字符串
来源：http://dmd.quarkkingdee.top

Py:   "ab" * 3
来源：http://jec.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://vrd.uphjek.com

JS:   "ab".repeat(3)
来源：http://ivd.yj20258888.top

TS:   "ab".repeat(3)
来源：http://zoq.yuanzhike.top

Java: "ab".repeat(3)
来源：http://dqs.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://awc.hesvh.cn

Ruby: "ab" * 3
来源：http://yce.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fji.jqgufenzy.top

[E03] 截取子串
来源：http://rhv.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://csx.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uga.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xhz.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://ciw.hnqzz.top

Java: s.substring(1, 4)
来源：http://rdl.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tbx.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://siz.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://bjw.zycfv.cn

[E04] 查找子串位置
来源：http://ykg.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://xcj.bjfxy.top


<!-- 参考信息 -->