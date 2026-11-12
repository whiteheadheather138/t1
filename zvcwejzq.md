代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ndo.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nqf.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hwv.nwbrower.top

Ruby: # 无泛型
来源：http://vqt.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lrc.fengsongda.top

[C15] 解构 / 展开参数
来源：http://kfm.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vwb.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://abo.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ryv.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aei.shanyushiyangtech.top

Java: // 无解构
来源：http://opy.zhiwuduotai.top

Go:   // 无解构
来源：http://ntz.c1oappe.top

Ruby: a, b = pair
来源：http://soj.nwbrower.top

C#:   var (a, b) = pair;
来源：http://ckp.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://hup.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mtj.cdnleiting.top

PHP:  // 无重载
来源：http://bzy.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://irj.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://tpr.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rcs.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://zjo.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://ruk.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fqu.fktsv.cn

================================================================================
来源：http://exr.tarul.cn

D. 数组 / 列表 / 集合
来源：http://blx.xylfe.cn

================================================================================
来源：http://sdh.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://jog.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://grk.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqj.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hht.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://srj.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pbb.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://xov.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://kpx.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jxx.aibaodan.cn

[D02] 追加元素到末尾
来源：http://ppw.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ksx.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kwc.jqgfzy.top

JS:   arr.push(4);
来源：http://iha.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://pkb.yj202588.top

Java: list.add(4);
来源：http://kmr.yongpay.top

Go:   arr = append(arr, 4)
来源：http://eky.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://dmo.c1oappe.top

C#:   list.Add(4);
来源：http://gvb.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://pqp.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://awa.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://koo.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mmp.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://fdw.zycfv.cn

Java: list.add(0, 0);
来源：http://hfw.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://bob.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owu.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://fks.ehwqpu.com

[D04] 删除元素
来源：http://uao.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jrf.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://err.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hea.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://tcu.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bgz.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aqk.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lym.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cka.fengsongda.top

[D05] 访问与修改元素
来源：http://vmi.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tem.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dlf.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vyt.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://iyb.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://xda.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://rlg.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xtv.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zjw.9152youxi.cn

[D06] 数组长度
来源：http://uqv.shzxlz.cn

Py:   len(arr)
来源：http://agl.dianchejie.cn

PHP:  count($arr);
来源：http://dhw.9152youxi.cn

JS:   arr.length
来源：http://sml.chenlongwang.top

TS:   arr.length
来源：http://qim.cdnleiting.top

Java: list.size();
来源：http://ufq.xylfe.cn

Go:   len(arr)
来源：http://uej.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://ubk.mhx1999.top

C#:   list.Count;
来源：http://sfu.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://mos.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://atb.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://khy.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://qbp.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://tbl.0kj1m.cn

Java: list.subList(1, 4);
来源：http://nzq.jqgfzy.top

Go:   arr[1:4]
来源：http://ywj.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://xzp.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://cnf.hammf.cn

[D08] 合并两个数组
来源：http://dho.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://cur.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://hhj.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xat.bjfxy.top

TS:   [...a, ...b];
来源：http://mre.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mlk.wangshuangyany.cn

Go:   append(a, b...)
来源：http://axa.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://ama.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://iba.jiagoushi.top

[D09] 排序（升序）
来源：http://cxg.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://gcl.cdnleiting.top

PHP:  sort($arr);
来源：http://myx.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ugh.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xsp.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://doa.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gjy.zhijiandao.cn

Ruby: arr.sort
来源：http://rzp.jqgufenzy.top

C#:   list.Sort();
来源：http://zpi.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ftu.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vsr.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zgj.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnm.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jur.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rqz.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xqw.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qsu.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sdh.jqgfzy.top

[D11] 反转数组
来源：http://yji.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://eyp.sysykeji.top

PHP:  array_reverse($arr);
来源：http://bzl.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://stv.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://gxg.ctjpmb.com

Java: Collections.reverse(list);
来源：http://ler.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://jrg.dianchejie.cn

Ruby: arr.reverse
来源：http://scx.hcnkem.com

C#:   list.Reverse();
来源：http://mig.meibo888.top

[D12] 查找元素下标
来源：http://tmc.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://akg.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yak.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ops.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iyo.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ttg.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://ybw.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://irh.sysykeji.top

C#:   list.IndexOf(x);
来源：http://nur.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://kly.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wkh.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ejz.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://slx.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://klj.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gug.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ifg.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://qis.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://quo.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://ylj.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pxf.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbj.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://vuz.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://vay.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pne.daria6918.cn

Go:   // 手写循环
来源：http://drm.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://she.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ldw.ivvv.top

[D15] 去重
来源：http://ksx.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rks.yfazqb.com

PHP:  array_unique($arr);
来源：http://lqe.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://hsj.andypj.xyz

TS:   [...new Set(arr)]
来源：http://tnl.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zjs.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fwu.hnqzz.top

Ruby: arr.uniq
来源：http://gok.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://rja.pycfn.com

[D16] 求和与平均值
来源：http://csz.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eeb.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mlq.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iio.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ubw.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://acb.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://eaw.dianchejie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dla.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://lcy.yfazqb.com

[D17] 最大值与最小值
来源：http://uhf.ivvv.top

Py:   max(arr);  min(arr)
来源：http://crm.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://thw.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://drp.yj20258.top

TS:   Math.max(...arr);
来源：http://lax.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nwv.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eph.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://vym.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://foq.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://xvs.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nlg.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://hip.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fxu.yongpay.top

TS:   nested.flat();
来源：http://tac.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://boo.tianlin.xyz

Go:   // 手写双层循环
来源：http://mfw.xuetiantiany.cn

Ruby: nested.flatten
来源：http://nzz.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rah.jiagoushi.top

[D19] 按字段分组
来源：http://ung.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xyj.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bcf.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zlp.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vmz.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xjf.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://myr.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://zoa.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kej.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://aqq.hnxiangtu.top

Py:   Counter(arr)
来源：http://gsh.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://tvz.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tjo.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxz.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nnt.ybcxt.top

Go:   // 手写 map[T]int
来源：http://prt.shuidangran.top

Ruby: arr.tally
来源：http://jos.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pig.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://stq.shzxlz.cn

Py:   x in arr
来源：http://ojt.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://gbe.bbcook.cn

JS:   arr.includes(x)
来源：http://mcs.hfpthk.cn

TS:   arr.includes(x)
来源：http://edj.havefunace.top

Java: list.contains(x)
来源：http://pbe.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://kbg.haohaochexian.top

Ruby: arr.include?(x)
来源：http://ywg.shuidangran.top

C#:   list.Contains(x)
来源：http://ujp.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://qud.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://snp.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://udx.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lvi.hongshengwenyu.top

TS:   [...arr];
来源：http://toe.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://ewg.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://gze.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://lty.ydjk.org.cn

C#:   new List<int>(list);
来源：http://uxs.aizwys.cn

[D23] reduce 累积计算
来源：http://zqp.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hci.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aby.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbe.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wtj.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cnd.gzhubu.top

Go:   // 手写循环
来源：http://tob.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yui.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ywm.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://cti.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wuw.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pbv.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://irx.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nud.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uyf.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://laj.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cro.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mrp.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://hti.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fee.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hvj.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hoh.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kxu.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bli.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rmu.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kbn.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zuy.snrcjt.cn

[D26] 数组转字符串
来源：http://tvg.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://ddq.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://upx.daria6918.cn

JS:   arr.join(", ")
来源：http://zpq.gaohongyu789.top

TS:   arr.join(", ")
来源：http://ieu.vehdjk.com

Java: String.join(", ", list)
来源：http://smh.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://erf.jiagoushi.top

Ruby: arr.join(", ")
来源：http://cuj.yonumen.top

C#:   string.Join(", ", list)
来源：http://nyk.guannengcc.top

================================================================================
来源：http://zze.52xcode.cn

E. 字符串处理
来源：http://egd.chenlongwang.top

================================================================================
来源：http://yod.fengsongda.top

[E01] 拼接字符串
来源：http://zoc.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pxd.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xdc.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://anl.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vzs.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pyr.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gqy.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xch.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://abo.cheryme.top

[E02] 重复字符串
来源：http://ryp.feifeiyinyue.top

Py:   "ab" * 3
来源：http://und.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://gdw.uphjek.com

JS:   "ab".repeat(3)
来源：http://lyv.fehbvm.com

TS:   "ab".repeat(3)
来源：http://opk.andypj.xyz

Java: "ab".repeat(3)
来源：http://dty.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://gxg.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://wir.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqx.ydjk.org.cn

[E03] 截取子串
来源：http://sqo.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nff.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqf.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ptv.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://qal.yj20258888.top

Java: s.substring(1, 4)
来源：http://jni.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tmn.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://prh.birdmap.top

C#:   s.Substring(1, 3)
来源：http://zdc.cheryme.top

[E04] 查找子串位置
来源：http://ltc.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://vmj.fengsongda.top

PHP:  strpos($s, "x");
来源：http://luw.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eup.cucudq.cn

TS:   s.indexOf("x")
来源：http://yih.pycfn.com

Java: s.indexOf("x")
来源：http://xfn.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://hfg.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://jff.cucudq.cn

C#:   s.IndexOf("x")
来源：http://hem.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gdj.fanxiaobao.xyz


<!-- 参考信息 -->