代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lzl.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqo.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qyg.chenlongwang.top

Ruby: # 无泛型
来源：http://aiq.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lom.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://lia.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://stb.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://mfx.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://twn.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zoi.jiagoushi.top

Java: // 无解构
来源：http://hso.dashuyun.cn

Go:   // 无解构
来源：http://boq.ybcxt.top

Ruby: a, b = pair
来源：http://saa.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://zlr.yj202588.top

[C16] 函数 / 方法重载
来源：http://fzy.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vtr.jinqigfzy.top

PHP:  // 无重载
来源：http://hvk.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://jlu.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://yjw.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iag.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://qus.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://vlb.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rxx.zycfv.cn

================================================================================
来源：http://cdm.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://cqt.zdqjudy.top

================================================================================
来源：http://vma.sxryk.cn

[D01] 创建数组 / 列表
来源：http://wvj.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwd.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://apr.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mat.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://ahp.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sqv.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://vyb.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://rjl.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kxe.shzxlz.cn

[D02] 追加元素到末尾
来源：http://qyb.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ujq.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zxl.nanxuanxn.top

JS:   arr.push(4);
来源：http://ahd.havefunace.top

TS:   arr.push(4);
来源：http://ryt.tanke756.top

Java: list.add(4);
来源：http://pwv.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://xwc.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://dly.hfpthk.cn

C#:   list.Add(4);
来源：http://zsi.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://nhw.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://hbl.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fiq.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cts.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://bqk.fzhhl.top

Java: list.add(0, 0);
来源：http://vmp.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://drn.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ydi.cheryme.top

C#:   list.Insert(0, 0);
来源：http://gpg.zhixingplan.top

[D04] 删除元素
来源：http://bfg.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hzy.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qrn.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gjn.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://yxz.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qyo.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jnn.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zuz.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kii.0kj1m.cn

[D05] 访问与修改元素
来源：http://vhk.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mmu.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aph.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ssc.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://udp.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://vtd.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://gai.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tdq.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nnb.pycfn.com

[D06] 数组长度
来源：http://qms.ybcxt.top

Py:   len(arr)
来源：http://oqo.birdmap.top

PHP:  count($arr);
来源：http://wxp.ehwqpu.com

JS:   arr.length
来源：http://kdm.wangshuangyany.cn

TS:   arr.length
来源：http://mtu.zycfv.cn

Java: list.size();
来源：http://xix.kuanghao11.cn

Go:   len(arr)
来源：http://nyw.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://oxn.hfpthk.cn

C#:   list.Count;
来源：http://nvn.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://ycw.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ocb.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qpy.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://gum.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://bej.tianlin.xyz

Java: list.subList(1, 4);
来源：http://fig.zycfv.cn

Go:   arr[1:4]
来源：http://jau.svipenyu.cn

Ruby: arr[1, 3]
来源：http://sie.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://grs.chenzaomai.com

[D08] 合并两个数组
来源：http://zrm.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://ycb.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://smh.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mlv.nanxuanxn.top

TS:   [...a, ...b];
来源：http://lul.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jhk.jyoumei.cn

Go:   append(a, b...)
来源：http://bun.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://ebd.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://jkl.zhijiandao.cn

[D09] 排序（升序）
来源：http://sjb.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xgv.iojbl.cn

PHP:  sort($arr);
来源：http://cox.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zwk.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hly.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jst.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rzj.chenzaomai.com

Ruby: arr.sort
来源：http://gva.cheryme.top

C#:   list.Sort();
来源：http://irk.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jsw.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jte.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vev.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cuk.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://efo.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xms.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lwo.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lph.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://trl.kuanghao11.cn

[D11] 反转数组
来源：http://jkf.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://tqa.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://aog.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sfh.jianghu66.top

TS:   [...arr].reverse();
来源：http://fop.tanke756.top

Java: Collections.reverse(list);
来源：http://rhr.havefunace.top

Go:   slices.Reverse(arr)
来源：http://ajl.tanke756.top

Ruby: arr.reverse
来源：http://wjt.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://iqy.cashguo.top

[D12] 查找元素下标
来源：http://ejx.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://voa.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ijd.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qzg.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emi.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yus.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://pdq.redwolf501.top

Ruby: arr.index(x)
来源：http://mcw.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://lcm.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://gkl.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://irg.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syx.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://wrp.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://mgn.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rnl.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tvz.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ftc.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://kxk.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://maz.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://snn.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fne.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://zwj.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://ypd.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zqp.birdmap.top

Go:   // 手写循环
来源：http://lbg.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://dsh.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eyi.fktsv.cn

[D15] 去重
来源：http://mly.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gbj.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://arl.fktsv.cn

JS:   [...new Set(arr)]
来源：http://jeu.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://oei.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tgl.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://efm.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://bqc.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://tml.c1oappe.top

[D16] 求和与平均值
来源：http://etu.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://umn.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://apb.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iwb.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fsc.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nen.0kj1m.cn

Go:   // 手写循环累加
来源：http://cfl.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yum.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://fvr.zdqjudy.top

[D17] 最大值与最小值
来源：http://muc.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://ezv.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://ejd.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ppx.zycfv.cn

TS:   Math.max(...arr);
来源：http://gkz.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wbo.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ieq.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://zux.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://cat.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://kba.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pwh.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://xsi.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fcb.bjfxy.top

TS:   nested.flat();
来源：http://ios.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nkb.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://qfj.yj20258888.top

Ruby: nested.flatten
来源：http://abp.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yoe.havefunace.top

[D19] 按字段分组
来源：http://lgu.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pxn.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gku.jlsjyb.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kdr.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nob.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzq.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://tpf.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cyz.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zia.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://lfa.aizwys.cn

Py:   Counter(arr)
来源：http://hlp.yuxming.cn

PHP:  array_count_values($arr);
来源：http://mwt.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yve.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ely.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kmu.sysykeji.top

Go:   // 手写 map[T]int
来源：http://kyc.0kj1m.cn

Ruby: arr.tally
来源：http://jfr.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://utu.epnwcf.com

[D21] 判断是否包含某元素
来源：http://wrk.c1oappe.top

Py:   x in arr
来源：http://njr.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://svm.yonumen.top

JS:   arr.includes(x)
来源：http://ixr.hcnkem.com

TS:   arr.includes(x)
来源：http://nom.uphjek.com

Java: list.contains(x)
来源：http://wbu.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://gbk.aizwys.cn

Ruby: arr.include?(x)
来源：http://pgk.shuidangran.top

C#:   list.Contains(x)
来源：http://iqb.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://opv.shzxlz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wik.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dzi.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://smg.hongshengwenyu.top

TS:   [...arr];
来源：http://enj.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://skk.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://mrs.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://yqq.vehdjk.com

C#:   new List<int>(list);
来源：http://axe.cqqwz.cn

[D23] reduce 累积计算
来源：http://ynb.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgn.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odo.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://avo.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dmz.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ter.chenzaomai.com

Go:   // 手写循环
来源：http://hzd.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dcr.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gam.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://flr.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kie.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://var.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ejt.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bmp.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnp.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://njx.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rbp.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fcs.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://zir.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://usu.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udb.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hjk.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wbe.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cgd.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gls.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kmj.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqz.bjfxy.top

[D26] 数组转字符串
来源：http://vbx.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://deq.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://ctg.yanxiufei.cn

JS:   arr.join(", ")
来源：http://tlu.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://qan.jinqigufen.top

Java: String.join(", ", list)
来源：http://teo.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://swp.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://dzu.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://rqt.yanxiufei.cn

================================================================================
来源：http://auk.hammf.cn

E. 字符串处理
来源：http://inm.jiagoushi.top

================================================================================
来源：http://xkc.cdnleiting.top

[E01] 拼接字符串
来源：http://yvg.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://icj.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qbf.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzh.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pka.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sas.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lvj.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dlk.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://epq.zhongyouzk.top

[E02] 重复字符串
来源：http://gnw.52xcode.cn

Py:   "ab" * 3
来源：http://umu.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://dhm.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://zsu.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://isc.wangdashe.top

Java: "ab".repeat(3)
来源：http://cax.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://dpi.c1oappe.top

Ruby: "ab" * 3
来源：http://nol.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vka.bbcook.cn

[E03] 截取子串
来源：http://hsw.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://upf.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://equ.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xee.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://yft.hammf.cn

Java: s.substring(1, 4)
来源：http://wsl.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nsr.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wtr.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://pqy.fehbvm.com

[E04] 查找子串位置
来源：http://rme.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://sfn.tarul.cn

PHP:  strpos($s, "x");
来源：http://tfk.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://era.daxiang520.top

TS:   s.indexOf("x")
来源：http://aus.dashuyun.cn

Java: s.indexOf("x")
来源：http://hxu.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://yrh.ctjpmb.com

Ruby: s.index("x")
来源：http://wtu.daria6918.cn

C#:   s.IndexOf("x")
来源：http://bzy.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ntc.haohaochexian.top


<!-- 参考信息 -->