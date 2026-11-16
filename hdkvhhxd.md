代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://awv.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kkj.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://luf.ybcxt.top

Ruby: # 无泛型
来源：http://zeo.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nrl.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://acy.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aoi.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://keb.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ccp.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rob.316326.xyz

Java: // 无解构
来源：http://tln.zdbjq.cn

Go:   // 无解构
来源：http://vra.daria6918.cn

Ruby: a, b = pair
来源：http://qjg.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://bav.epnwcf.com

[C16] 函数 / 方法重载
来源：http://pnf.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://frv.ppjwa.cn

PHP:  // 无重载
来源：http://xoe.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wmj.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://pyh.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ubg.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://dqt.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://ykr.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://woo.dianchejie.cn

================================================================================
来源：http://lis.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://mpa.fehbvm.com

================================================================================
来源：http://edy.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://gvn.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gzt.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ocw.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bkl.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pxl.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bdr.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://xwy.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://rto.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sld.chenlongwang.top

[D02] 追加元素到末尾
来源：http://mox.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aos.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ouv.cdnleiting.top

JS:   arr.push(4);
来源：http://mvd.cheryme.top

TS:   arr.push(4);
来源：http://wtb.nanxuanxn.top

Java: list.add(4);
来源：http://nsx.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://dki.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://pai.xziqi.cn

C#:   list.Add(4);
来源：http://lwu.epnwcf.com

[D03] 在指定位置插入元素
来源：http://raj.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://xwx.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://edc.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fsm.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://txf.pycfn.com

Java: list.add(0, 0);
来源：http://tkw.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://rvl.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nua.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://rue.hongshengwenyu.top

[D04] 删除元素
来源：http://tkr.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fxc.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cgh.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iri.havefunace.top

TS:   arr.splice(0, 1);
来源：http://mss.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hxb.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hfo.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://exa.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wlg.nanxuanxn.top

[D05] 访问与修改元素
来源：http://tid.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://myr.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hgv.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xfy.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://itu.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://gff.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://gtq.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dxp.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://okc.daria6918.cn

[D06] 数组长度
来源：http://xzw.cheryme.top

Py:   len(arr)
来源：http://wdb.tianlin.xyz

PHP:  count($arr);
来源：http://wxt.yuxming.cn

JS:   arr.length
来源：http://jdw.fzhhl.top

TS:   arr.length
来源：http://kqn.smart0.xyz

Java: list.size();
来源：http://otk.ydjk.org.cn

Go:   len(arr)
来源：http://vpo.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://ybe.yangfankeji.com

C#:   list.Count;
来源：http://ugf.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://klz.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pfj.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://yvs.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://kom.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://iwe.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://jrs.zhixingplan.top

Go:   arr[1:4]
来源：http://vyw.cucudq.cn

Ruby: arr[1, 3]
来源：http://toh.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://tdl.316326.xyz

[D08] 合并两个数组
来源：http://iir.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://gyo.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://vhw.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://pny.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://gjh.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jlu.xuetiantiany.cn

Go:   append(a, b...)
来源：http://flz.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://mos.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://hgq.feifeiyinyue.top

[D09] 排序（升序）
来源：http://etq.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://iqn.zhengqikj.top

PHP:  sort($arr);
来源：http://gjp.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hrf.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gcs.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vrp.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nfk.haohaochexian.top

Ruby: arr.sort
来源：http://yek.cqqwz.cn

C#:   list.Sort();
来源：http://qag.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dwl.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://han.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hbd.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yea.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mag.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ybm.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fcl.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://btp.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kdq.shanyushiyangkeji.top

[D11] 反转数组
来源：http://cjv.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mqb.ydzc1.top

PHP:  array_reverse($arr);
来源：http://xmp.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fex.cucudq.cn

TS:   [...arr].reverse();
来源：http://rxj.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://flk.sweek.top

Go:   slices.Reverse(arr)
来源：http://aqm.vqdsnc.cn

Ruby: arr.reverse
来源：http://myk.pengpengdd.cyou

C#:   list.Reverse();
来源：http://cyz.c1oappe.top

[D12] 查找元素下标
来源：http://oeu.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://sit.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xdk.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rir.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lmz.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vix.pycfn.com

Go:   slices.Index(arr, x)
来源：http://whl.zhoulong.xyz

Ruby: arr.index(x)
来源：http://zdp.hnqzz.top

C#:   list.IndexOf(x);
来源：http://hml.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://ftb.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hpr.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eix.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://qzo.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://sei.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://itv.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odo.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://imf.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wfj.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://mxv.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iea.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zrd.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://egq.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://bvx.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rxv.sysykeji.top

Go:   // 手写循环
来源：http://yde.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://atw.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ksn.bbcook.cn

[D15] 去重
来源：http://nwy.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bpp.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://lyl.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://yph.hnqzz.top

TS:   [...new Set(arr)]
来源：http://dia.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qcn.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jmw.sufxvd.cn

Ruby: arr.uniq
来源：http://ntb.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://apf.ybcxt.top

[D16] 求和与平均值
来源：http://wnb.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qgz.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tpf.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybw.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mzw.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wmn.chenzaomai.com

Go:   // 手写循环累加
来源：http://bvc.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rbn.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://mas.vqdsnc.cn

[D17] 最大值与最小值
来源：http://zoi.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://yxn.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://qec.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://prw.zdqjudy.top

TS:   Math.max(...arr);
来源：http://pok.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kbv.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://akz.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://jgd.meibo888.top

C#:   list.Max();  list.Min()
来源：http://uvb.pycfn.com

[D18] 扁平化嵌套数组
来源：http://tai.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://efu.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://mbi.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wmz.cheryme.top

TS:   nested.flat();
来源：http://zxv.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vpv.yanxiufei.cn

Go:   // 手写双层循环
来源：http://dxy.sjlbkw.cn

Ruby: nested.flatten
来源：http://atn.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oxg.xuanzx.com

[D19] 按字段分组
来源：http://ric.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nuw.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vts.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://shc.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bcu.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://caj.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://xqx.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xdh.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tgx.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://smm.zhengqikj.top

Py:   Counter(arr)
来源：http://wuy.wangdashe.top

PHP:  array_count_values($arr);
来源：http://ooi.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qtt.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdl.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kdg.fengsongda.top

Go:   // 手写 map[T]int
来源：http://vqp.daria6918.cn

Ruby: arr.tally
来源：http://xho.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jmu.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://nij.cqqwz.cn

Py:   x in arr
来源：http://pde.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://bzb.zdqjudy.top

JS:   arr.includes(x)
来源：http://njf.pycfn.com

TS:   arr.includes(x)
来源：http://clj.xuanzx.com

Java: list.contains(x)
来源：http://liz.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://riy.ppjwa.cn

Ruby: arr.include?(x)
来源：http://qwm.yj202588.top

C#:   list.Contains(x)
来源：http://gzy.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://jlt.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pcl.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ouu.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cxw.wangdashe.top

TS:   [...arr];
来源：http://aem.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://vrg.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://kjw.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://iwa.xuanzx.com

C#:   new List<int>(list);
来源：http://uer.jianghu66.top

[D23] reduce 累积计算
来源：http://faj.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sqb.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wuy.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvh.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upt.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vhz.yanxiufei.cn

Go:   // 手写循环
来源：http://ejk.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jkk.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sjr.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://lvt.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wwh.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bdk.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ucl.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hei.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://elk.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ngw.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://phg.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejo.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://gom.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blg.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oyx.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lym.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hmu.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vlb.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kra.hongshengwenyu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ggc.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uwj.sufxvd.cn

[D26] 数组转字符串
来源：http://erw.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://aky.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://fdb.hesvh.cn

JS:   arr.join(", ")
来源：http://vjy.epnwcf.com

TS:   arr.join(", ")
来源：http://cso.redwolf501.top

Java: String.join(", ", list)
来源：http://qel.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://dxq.yfazqb.com

Ruby: arr.join(", ")
来源：http://qcj.xuanzx.com

C#:   string.Join(", ", list)
来源：http://eyg.zhixingplan.top

================================================================================
来源：http://zhp.jinqigufen.top

E. 字符串处理
来源：http://tew.xingfuxueyuan.xyz

================================================================================
来源：http://phv.zhoulong.xyz

[E01] 拼接字符串
来源：http://jhe.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://svf.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://asa.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbv.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pgl.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jgl.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tbi.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hfq.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://evh.guowangkeji.top

[E02] 重复字符串
来源：http://xyj.xuetiantiany.cn

Py:   "ab" * 3
来源：http://clw.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://xih.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://qsr.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://glv.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://veb.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://zzx.dashuyun.cn

Ruby: "ab" * 3
来源：http://wze.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mmg.fktsv.cn

[E03] 截取子串
来源：http://aer.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sxf.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kyl.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mlb.xinyue.icu

TS:   s.slice(1, 4)
来源：http://vrm.jqgfzy.top

Java: s.substring(1, 4)
来源：http://szm.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbo.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://lot.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://fee.hnqzz.top

[E04] 查找子串位置
来源：http://prc.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://wnw.smart0.xyz

PHP:  strpos($s, "x");
来源：http://xdl.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lmt.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://okm.yuanzhike.top

Java: s.indexOf("x")
来源：http://rwv.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://adg.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://aqi.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://mlq.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ehn.smart0.xyz


<!-- 参考信息 -->