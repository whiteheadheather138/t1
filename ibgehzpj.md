代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qdz.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pmu.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://euk.cucudq.cn

Ruby: # 无泛型
来源：http://xvf.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://urm.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://kva.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eho.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://pzs.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ehc.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://efk.haohaochexian.top

Java: // 无解构
来源：http://iwj.wangshuangyany.cn

Go:   // 无解构
来源：http://zou.yueranfly.top

Ruby: a, b = pair
来源：http://flc.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://lep.hammf.cn

[C16] 函数 / 方法重载
来源：http://gqf.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://neb.dashuyun.cn

PHP:  // 无重载
来源：http://pha.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ovu.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://qxw.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pdn.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://omz.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://vvh.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://blq.smart0.xyz

================================================================================
来源：http://psu.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://ljp.ywan-chungtsiang.top

================================================================================
来源：http://xjd.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://veh.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qff.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ptd.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sqh.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://djo.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://war.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://xsj.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://fqt.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://epf.chenlongwang.top

[D02] 追加元素到末尾
来源：http://tux.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xot.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xtx.jianghu66.top

JS:   arr.push(4);
来源：http://bbb.ydjk.org.cn

TS:   arr.push(4);
来源：http://dmi.feifeiyinyue.top

Java: list.add(4);
来源：http://pvm.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://rah.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://luc.cqqwz.cn

C#:   list.Add(4);
来源：http://ybw.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://bcl.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://zbt.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pou.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ywg.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://rep.tanke756.top

Java: list.add(0, 0);
来源：http://bdt.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vdo.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dwl.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://esw.hysaishi.cn

[D04] 删除元素
来源：http://sur.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hai.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sxf.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dsf.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://lmo.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://szr.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hep.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://epm.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://csb.jiagoushi.top

[D05] 访问与修改元素
来源：http://yry.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tmi.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xpi.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lwr.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://jsj.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://vzs.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://zlm.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bpr.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://opg.mhx1999.top

[D06] 数组长度
来源：http://xkk.ehwqpu.com

Py:   len(arr)
来源：http://nio.ivvv.top

PHP:  count($arr);
来源：http://rgt.aibaodan.cn

JS:   arr.length
来源：http://dtt.gogol.net.cn

TS:   arr.length
来源：http://lfi.fengsongda.top

Java: list.size();
来源：http://zdt.zhongyouzk.top

Go:   len(arr)
来源：http://jom.smart0.xyz

Ruby: arr.length; arr.size
来源：http://zyl.zhaomingkeji.xyz

C#:   list.Count;
来源：http://csx.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://iia.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vog.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rbp.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://vpd.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://idx.yuanzhike.top

Java: list.subList(1, 4);
来源：http://dgy.jyoumei.cn

Go:   arr[1:4]
来源：http://tpu.uphjek.com

Ruby: arr[1, 3]
来源：http://vir.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://zgx.ydzc1.top

[D08] 合并两个数组
来源：http://qhe.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://fam.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://ytv.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://llg.hysaishi.cn

TS:   [...a, ...b];
来源：http://gvc.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kwt.c1oappe.top

Go:   append(a, b...)
来源：http://ouk.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://gee.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://qrg.52xcode.cn

[D09] 排序（升序）
来源：http://lrl.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://jyt.sufxvd.cn

PHP:  sort($arr);
来源：http://vzk.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rrf.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fml.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bni.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tfy.jiagoushi.top

Ruby: arr.sort
来源：http://obe.xziqi.cn

C#:   list.Sort();
来源：http://imh.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vlo.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rrs.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxk.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hwx.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ehl.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://scl.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ccx.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ssj.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wgp.redwolf501.top

[D11] 反转数组
来源：http://khx.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://gae.tanke756.top

PHP:  array_reverse($arr);
来源：http://aam.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://quh.jinqigufen.top

TS:   [...arr].reverse();
来源：http://bnu.mhx1999.top

Java: Collections.reverse(list);
来源：http://itg.sysykeji.top

Go:   slices.Reverse(arr)
来源：http://bgx.xylfe.cn

Ruby: arr.reverse
来源：http://qha.sxryk.cn

C#:   list.Reverse();
来源：http://cjp.jianghu66.top

[D12] 查找元素下标
来源：http://chg.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://uug.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hjl.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgs.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfs.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dfv.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://xko.mhx1999.top

Ruby: arr.index(x)
来源：http://mst.uphjek.com

C#:   list.IndexOf(x);
来源：http://swj.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://pxf.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rwj.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cgc.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://poh.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://pkr.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://urp.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yvu.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uxs.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tar.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://hra.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ruz.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://utz.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://nvp.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://neu.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://urg.epnwcf.com

Go:   // 手写循环
来源：http://yto.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mzg.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aff.ivvv.top

[D15] 去重
来源：http://eac.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wcu.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://opv.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://bwz.guannengcc.top

TS:   [...new Set(arr)]
来源：http://egz.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://akn.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://jzt.tarul.cn

Ruby: arr.uniq
来源：http://nxh.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://zhv.tarul.cn

[D16] 求和与平均值
来源：http://bdd.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hdt.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dtm.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sta.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vli.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jzg.dianchejie.cn

Go:   // 手写循环累加
来源：http://ykr.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wfe.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://aks.guowangkeji.top

[D17] 最大值与最小值
来源：http://nsq.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://qns.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://nvi.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxi.yj20258.top

TS:   Math.max(...arr);
来源：http://uxc.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ieq.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aiy.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://xyb.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://uke.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://qbw.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://srm.pycfn.com

PHP:  array_merge(...$nested);
来源：http://pqa.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fel.ydjk.org.cn

TS:   nested.flat();
来源：http://lct.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aqa.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://juv.yuanzhike.top

Ruby: nested.flatten
来源：http://sjv.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ccw.jqgufenzy.top

[D19] 按字段分组
来源：http://eyq.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://okz.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zrm.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://czg.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kpc.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gpg.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://jnd.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://phq.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lqw.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://twf.yonumen.top

Py:   Counter(arr)
来源：http://zpu.yj202588.top

PHP:  array_count_values($arr);
来源：http://gat.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atv.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cfa.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pcr.cashguo.top

Go:   // 手写 map[T]int
来源：http://gsu.vehdjk.com

Ruby: arr.tally
来源：http://tuq.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://miv.yongpay.top

[D21] 判断是否包含某元素
来源：http://soy.xingfuxueyuan.xyz

Py:   x in arr
来源：http://leq.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://jad.yongpay.top

JS:   arr.includes(x)
来源：http://die.yueranfly.top

TS:   arr.includes(x)
来源：http://tqt.daria6918.cn

Java: list.contains(x)
来源：http://vty.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://kho.tianlin.xyz

Ruby: arr.include?(x)
来源：http://mrp.hnqzz.top

C#:   list.Contains(x)
来源：http://jmr.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://fzg.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zew.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://var.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wlb.meibo888.top

TS:   [...arr];
来源：http://qgg.xziqi.cn

Java: new ArrayList<>(list);
来源：http://tvr.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://dmc.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://ixx.gogol.net.cn

C#:   new List<int>(list);
来源：http://lif.zhoulong.xyz

[D23] reduce 累积计算
来源：http://bde.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://etg.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rsr.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cra.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwm.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rsj.sufxvd.cn

Go:   // 手写循环
来源：http://jua.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hed.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mbg.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://edd.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://seo.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sqx.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hjr.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vzp.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zyc.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tux.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hag.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vtx.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://usu.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bqc.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xow.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cza.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rxb.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gtq.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ojw.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bnv.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xeb.epnwcf.com

[D26] 数组转字符串
来源：http://xyt.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://zvk.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://ewn.cqqwz.cn

JS:   arr.join(", ")
来源：http://clm.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://ral.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://zvl.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://qxh.cqqwz.cn

Ruby: arr.join(", ")
来源：http://kwd.smart0.xyz

C#:   string.Join(", ", list)
来源：http://rzl.zhiwuduotai.top

================================================================================
来源：http://agf.pycfn.com

E. 字符串处理
来源：http://iig.jqgufenzy.top

================================================================================
来源：http://ewn.yongpay.top

[E01] 拼接字符串
来源：http://olr.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tep.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tup.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yaz.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nuy.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nca.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://anp.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zqv.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ftq.9152youxi.cn

[E02] 重复字符串
来源：http://ttv.meibo888.top

Py:   "ab" * 3
来源：http://rcs.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://ity.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://via.sysykeji.top

TS:   "ab".repeat(3)
来源：http://rpy.nanxinkj.top

Java: "ab".repeat(3)
来源：http://rjy.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://ium.smart0.xyz

Ruby: "ab" * 3
来源：http://shu.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uhw.zdbjq.cn

[E03] 截取子串
来源：http://fyh.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hci.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://niy.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xel.yj20258888.top

TS:   s.slice(1, 4)
来源：http://uti.ctjpmb.com

Java: s.substring(1, 4)
来源：http://ghd.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eei.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ssu.havefunace.top

C#:   s.Substring(1, 3)
来源：http://kit.zdqjudy.top

[E04] 查找子串位置
来源：http://rly.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://tbr.ydzc1.top

PHP:  strpos($s, "x");
来源：http://luj.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bvi.dashuyun.cn

TS:   s.indexOf("x")
来源：http://nqg.c1oappe.top

Java: s.indexOf("x")
来源：http://qyn.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://dlu.iojbl.cn

Ruby: s.index("x")
来源：http://yhw.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://sci.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iuy.fzhhl.top


<!-- 参考信息 -->