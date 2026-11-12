代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gue.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pqq.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://irs.yuanzhike.top

Ruby: # 无泛型
来源：http://mau.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mah.mhx1999.top

[C15] 解构 / 展开参数
来源：http://syh.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dyy.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://ady.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ozv.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://njt.yuxming.cn

Java: // 无解构
来源：http://pyb.yj202588.top

Go:   // 无解构
来源：http://upo.yj20258.top

Ruby: a, b = pair
来源：http://bmo.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://lzi.daria6918.cn

[C16] 函数 / 方法重载
来源：http://jxh.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hgp.yuanzhike.top

PHP:  // 无重载
来源：http://ayl.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dzf.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://pio.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wov.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://lwv.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://vav.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hil.hammf.cn

================================================================================
来源：http://tev.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://bko.xziqi.cn

================================================================================
来源：http://owi.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://fhm.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sox.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vfp.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lxu.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ctt.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gpz.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://bbh.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://wqy.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lbz.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://jvt.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://urw.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lcv.uphjek.com

JS:   arr.push(4);
来源：http://gox.chenjidiqi.icu

TS:   arr.push(4);
来源：http://ewv.gzhubu.top

Java: list.add(4);
来源：http://rox.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://snz.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://zpx.mhx1999.top

C#:   list.Add(4);
来源：http://yao.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://wzc.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://nij.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yck.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ozh.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://sgp.bjfxy.top

Java: list.add(0, 0);
来源：http://dib.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://ktf.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sfc.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://bee.ydjk.org.cn

[D04] 删除元素
来源：http://mxt.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kvm.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vil.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gum.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://rxx.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mat.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qto.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dxi.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyc.zdbjq.cn

[D05] 访问与修改元素
来源：http://dis.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eag.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sbd.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wha.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mrs.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://iwc.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ujl.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ssc.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ldo.dianchejie.cn

[D06] 数组长度
来源：http://hfg.zhijiandao.cn

Py:   len(arr)
来源：http://amt.gogol.net.cn

PHP:  count($arr);
来源：http://iox.tianlin.xyz

JS:   arr.length
来源：http://dzx.yj20258888.top

TS:   arr.length
来源：http://sww.yj202588.top

Java: list.size();
来源：http://ykq.zdqjudy.top

Go:   len(arr)
来源：http://exi.guannengcc.top

Ruby: arr.length; arr.size
来源：http://vvl.nwbrower.top

C#:   list.Count;
来源：http://qxh.epnwcf.com

[D07] 切片 / 取子数组
来源：http://lud.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rwx.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://gxa.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://jml.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://boz.bbcook.cn

Java: list.subList(1, 4);
来源：http://cdc.jianghu66.top

Go:   arr[1:4]
来源：http://qiv.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://jqx.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://qdc.tianlin.xyz

[D08] 合并两个数组
来源：http://bll.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://aky.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://tai.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://riz.epnwcf.com

TS:   [...a, ...b];
来源：http://qsw.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nox.yvedp.cn

Go:   append(a, b...)
来源：http://blw.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://qsp.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://wmb.wangshuangyany.cn

[D09] 排序（升序）
来源：http://fou.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ruy.daxiang520.top

PHP:  sort($arr);
来源：http://bbw.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cuh.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nko.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lhy.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://akv.havefunace.top

Ruby: arr.sort
来源：http://bad.zdbjq.cn

C#:   list.Sort();
来源：http://aau.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eqi.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eee.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fkr.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bms.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://quy.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rnx.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxw.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nyc.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wgd.hnxiangtu.top

[D11] 反转数组
来源：http://bqx.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wzt.fengsongda.top

PHP:  array_reverse($arr);
来源：http://mxi.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gcf.yueranfly.top

TS:   [...arr].reverse();
来源：http://tuf.cucudq.cn

Java: Collections.reverse(list);
来源：http://emd.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://nza.chenzaomai.com

Ruby: arr.reverse
来源：http://kvg.jlsjyb.cn

C#:   list.Reverse();
来源：http://akt.pycfn.com

[D12] 查找元素下标
来源：http://olh.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://bfg.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fzr.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfk.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpm.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kap.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://wzd.hywenlv.cn

Ruby: arr.index(x)
来源：http://wbt.bbcook.cn

C#:   list.IndexOf(x);
来源：http://knd.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://nrn.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsj.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cnr.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://mjb.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://xuy.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vwf.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://taz.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://avp.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ucr.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://jtv.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rga.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xlb.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://vry.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://uiy.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://cij.jqgufenzy.top

Go:   // 手写循环
来源：http://ftg.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://btn.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://awo.gaohongyu789.top

[D15] 去重
来源：http://jex.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fsx.zycfv.cn

PHP:  array_unique($arr);
来源：http://kdp.guannengcc.top

JS:   [...new Set(arr)]
来源：http://uky.yvedp.cn

TS:   [...new Set(arr)]
来源：http://ywd.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fbn.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://obz.jyoumei.cn

Ruby: arr.uniq
来源：http://nuu.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://ety.chenzaomai.com

[D16] 求和与平均值
来源：http://pvs.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iuz.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nmu.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ovu.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdr.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mat.pycfn.com

Go:   // 手写循环累加
来源：http://nme.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qkp.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://cam.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://vmp.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://iqn.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://hqb.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iez.tian-w.cn

TS:   Math.max(...arr);
来源：http://goy.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yje.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fjz.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://uxn.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://wgv.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://lrr.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jpr.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://tdn.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dhr.tianlin.xyz

TS:   nested.flat();
来源：http://mme.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lhq.daria6918.cn

Go:   // 手写双层循环
来源：http://nmc.cucudq.cn

Ruby: nested.flatten
来源：http://kot.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hfl.zhoulong.xyz

[D19] 按字段分组
来源：http://seq.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rsh.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vdf.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mqr.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zry.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rsd.ivvv.top

Go:   // 手写 map[string][]T
来源：http://vjv.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://wdp.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://asm.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://kdj.hammf.cn

Py:   Counter(arr)
来源：http://qzf.wangdashe.top

PHP:  array_count_values($arr);
来源：http://eex.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://icq.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvw.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vyc.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://rww.vehdjk.com

Ruby: arr.tally
来源：http://spj.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://brx.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://ieu.yj202588.top

Py:   x in arr
来源：http://drd.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://bgv.xinyue.icu

JS:   arr.includes(x)
来源：http://soq.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://zrk.gaohongyu789.top

Java: list.contains(x)
来源：http://swb.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://idv.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://nuk.zhoulong.xyz

C#:   list.Contains(x)
来源：http://qcz.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://dae.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lei.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://obx.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bdp.316326.xyz

TS:   [...arr];
来源：http://zrk.jianghu66.top

Java: new ArrayList<>(list);
来源：http://svr.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vvx.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://frg.jqgufenzy.top

C#:   new List<int>(list);
来源：http://hdx.gotoacloud.top

[D23] reduce 累积计算
来源：http://eex.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pnl.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wlh.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpn.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hdg.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lwf.meibo888.top

Go:   // 手写循环
来源：http://uta.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nzy.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zfi.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://kwh.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://top.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xtu.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pss.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://noe.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofn.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vzd.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://snl.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dau.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://lqb.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cua.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jmd.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mtt.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rcu.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dxq.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://utc.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mzm.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lqm.quarkkingdee.top

[D26] 数组转字符串
来源：http://ghu.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://bdm.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://ubm.gaohongyu789.top

JS:   arr.join(", ")
来源：http://bdl.316326.xyz

TS:   arr.join(", ")
来源：http://ify.birdmap.top

Java: String.join(", ", list)
来源：http://gml.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://ouz.yuanzhike.top

Ruby: arr.join(", ")
来源：http://dfq.tarul.cn

C#:   string.Join(", ", list)
来源：http://rot.guowangkeji.top

================================================================================
来源：http://zlo.xylfe.cn

E. 字符串处理
来源：http://qdx.zhengqikj.top

================================================================================
来源：http://xqb.tanke756.top

[E01] 拼接字符串
来源：http://byj.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cos.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zli.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mec.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aya.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://foc.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ycw.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pdt.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nky.sxryk.cn

[E02] 重复字符串
来源：http://mfn.jqgfzy.top

Py:   "ab" * 3
来源：http://emi.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://tkr.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://hdc.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://zqf.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://dbr.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://dxj.guowangkeji.top

Ruby: "ab" * 3
来源：http://dgs.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iqd.sweek.top

[E03] 截取子串
来源：http://xlc.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ozy.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ytc.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cwl.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://fsv.xinyue.icu

Java: s.substring(1, 4)
来源：http://bkf.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wfw.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://uix.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://mkw.jiagoushi.top

[E04] 查找子串位置
来源：http://swh.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://zzg.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://tpg.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ebj.c1oappe.top

TS:   s.indexOf("x")
来源：http://ugt.hnqzz.top

Java: s.indexOf("x")
来源：http://geh.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://soc.ydzc1.top

Ruby: s.index("x")
来源：http://rvm.fengsongda.top

C#:   s.IndexOf("x")
来源：http://lvj.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vzk.yuanzhike.top


<!-- 参考信息 -->