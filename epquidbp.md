代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xji.uphjek.com

[C15] 解构 / 展开参数
来源：http://jwy.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hih.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://mwd.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jyt.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bwq.jyoumei.cn

Java: // 无解构
来源：http://fwp.gotoacloud.top

Go:   // 无解构
来源：http://jro.shzxlz.cn

Ruby: a, b = pair
来源：http://lrg.mhx1999.top

C#:   var (a, b) = pair;
来源：http://vtf.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://nax.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ido.yongpay.top

PHP:  // 无重载
来源：http://fdc.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hcf.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fww.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cxf.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://pzk.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://hsn.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cxd.xziqi.cn

================================================================================
来源：http://anz.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://uhh.jinghuilouyu.cn

================================================================================
来源：http://uku.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://fzs.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vzs.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qyc.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qlj.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rma.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qde.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://keb.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://ehj.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ijq.shuidangran.top

[D02] 追加元素到末尾
来源：http://jlz.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ovq.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tky.jianghu66.top

JS:   arr.push(4);
来源：http://cgq.cheryme.top

TS:   arr.push(4);
来源：http://tph.jlsjyb.cn

Java: list.add(4);
来源：http://ovy.hammf.cn

Go:   arr = append(arr, 4)
来源：http://ngv.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://wkx.bbcook.cn

C#:   list.Add(4);
来源：http://enx.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://wwn.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://onn.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aob.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zyb.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://gcd.cucudq.cn

Java: list.add(0, 0);
来源：http://zxd.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bsm.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qnr.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://rfc.andypj.xyz

[D04] 删除元素
来源：http://tfm.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gcb.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mng.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vep.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://avb.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uwz.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ada.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://upv.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mng.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://frr.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ncm.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jhn.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qlu.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://ptu.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ans.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://usp.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gcw.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vtk.dianchejie.cn

[D06] 数组长度
来源：http://rub.jqgfzy.top

Py:   len(arr)
来源：http://edx.aibaodan.cn

PHP:  count($arr);
来源：http://fmn.epnwcf.com

JS:   arr.length
来源：http://sev.fengsongda.top

TS:   arr.length
来源：http://mgn.birdmap.top

Java: list.size();
来源：http://ifr.jyoumei.cn

Go:   len(arr)
来源：http://paa.birdmap.top

Ruby: arr.length; arr.size
来源：http://nag.yongpay.top

C#:   list.Count;
来源：http://nwx.c1oappe.top

[D07] 切片 / 取子数组
来源：http://yky.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cpz.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://mod.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://psi.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://oio.redwolf501.top

Java: list.subList(1, 4);
来源：http://lis.cashguo.top

Go:   arr[1:4]
来源：http://kum.sweek.top

Ruby: arr[1, 3]
来源：http://zkf.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://lgn.zhixingplan.top

[D08] 合并两个数组
来源：http://xsx.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://snb.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://hio.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oqb.guowangkeji.top

TS:   [...a, ...b];
来源：http://ngz.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kzw.jinqigfzy.top

Go:   append(a, b...)
来源：http://dvk.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://iob.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://kff.jianghu66.top

[D09] 排序（升序）
来源：http://cyb.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://hmi.tanke756.top

PHP:  sort($arr);
来源：http://lkk.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mzy.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uag.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://hlt.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sek.hywenlv.cn

Ruby: arr.sort
来源：http://cqm.gzhubu.top

C#:   list.Sort();
来源：http://stz.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hpc.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pwn.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svc.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xbn.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqx.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wqc.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nvi.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bou.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://udq.sweek.top

[D11] 反转数组
来源：http://aqs.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fuh.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://sor.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://viq.ivvv.top

TS:   [...arr].reverse();
来源：http://izx.xylfe.cn

Java: Collections.reverse(list);
来源：http://kmv.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://byd.yueranfly.top

Ruby: arr.reverse
来源：http://dzh.xylfe.cn

C#:   list.Reverse();
来源：http://hbo.guowangkeji.top

[D12] 查找元素下标
来源：http://rfj.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://kvm.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tol.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxb.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nad.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tpg.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://fyt.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://atc.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://jxm.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://utb.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wtz.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hlm.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://lsv.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://yxu.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rox.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpu.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://jut.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ekq.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://srz.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jku.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ysq.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://ven.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://koj.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tge.dianchejie.cn

Go:   // 手写循环
来源：http://bok.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://gsv.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ufs.xziqi.cn

[D15] 去重
来源：http://bpw.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wao.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://ele.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://gny.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://xbu.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qwd.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xgt.ydjk.org.cn

Ruby: arr.uniq
来源：http://qws.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://hzy.shuidangran.top

[D16] 求和与平均值
来源：http://kkp.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wca.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ldt.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yad.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdf.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vol.hammf.cn

Go:   // 手写循环累加
来源：http://oxy.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yjo.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://qcw.bbcook.cn

[D17] 最大值与最小值
来源：http://txu.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://wld.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://fcp.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgw.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://vdc.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://swt.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wcd.cashguo.top

Ruby: arr.max;  arr.min
来源：http://nyk.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://dld.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://nrm.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ymn.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://lal.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vig.sufxvd.cn

TS:   nested.flat();
来源：http://ohv.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kea.haohaochexian.top

Go:   // 手写双层循环
来源：http://bhi.shzxlz.cn

Ruby: nested.flatten
来源：http://xmq.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmn.nanxuanxn.top

[D19] 按字段分组
来源：http://aod.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ble.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://skk.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zex.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqs.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pgh.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://pyl.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hmt.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://akq.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://ylt.uphjek.com

Py:   Counter(arr)
来源：http://pnj.tarul.cn

PHP:  array_count_values($arr);
来源：http://xvx.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hil.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pgk.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://apm.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://wbq.ctjpmb.com

Ruby: arr.tally
来源：http://fji.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dwq.cashguo.top

[D21] 判断是否包含某元素
来源：http://fxe.svipenyu.cn

Py:   x in arr
来源：http://fqb.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://yxh.jianghu66.top

JS:   arr.includes(x)
来源：http://xvq.daria6918.cn

TS:   arr.includes(x)
来源：http://hja.yuxming.cn

Java: list.contains(x)
来源：http://fcr.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://wbc.vehdjk.com

Ruby: arr.include?(x)
来源：http://dpv.zdqjudy.top

C#:   list.Contains(x)
来源：http://vjj.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://kmm.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kdq.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pzd.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mid.jqgufenzy.top

TS:   [...arr];
来源：http://tzm.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://pao.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://pxh.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://hos.9152youxi.cn

C#:   new List<int>(list);
来源：http://pfj.zycfv.cn

[D23] reduce 累积计算
来源：http://rad.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fpd.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tte.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvu.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znl.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rvn.tian-w.cn

Go:   // 手写循环
来源：http://whi.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgx.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lto.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://yuq.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jue.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tgb.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iom.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jhv.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://von.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rsm.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uxu.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://shl.meibo888.top

[D25] Set 集合去重与交并差
来源：http://cwv.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hff.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uny.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uls.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kyk.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yoz.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lxp.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jkv.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eys.birdmap.top

[D26] 数组转字符串
来源：http://mve.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://tmt.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://odc.9152youxi.cn

JS:   arr.join(", ")
来源：http://hdu.jinqigufen.top

TS:   arr.join(", ")
来源：http://fhk.wangdashe.top

Java: String.join(", ", list)
来源：http://rac.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://cce.fktsv.cn

Ruby: arr.join(", ")
来源：http://noe.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://zmh.daxiang520.top

================================================================================
来源：http://lod.feifeiyinyue.top

E. 字符串处理
来源：http://vpw.haohaochexian.top

================================================================================
来源：http://jso.c1oappe.top

[E01] 拼接字符串
来源：http://pjg.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lcp.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ygs.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ksc.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ljy.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sqv.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ppm.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yyy.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tzx.epnwcf.com

[E02] 重复字符串
来源：http://pdk.ppjwa.cn

Py:   "ab" * 3
来源：http://emz.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://avb.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://fwc.hammf.cn

TS:   "ab".repeat(3)
来源：http://ygm.0kj1m.cn

Java: "ab".repeat(3)
来源：http://anf.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://als.smart0.xyz

Ruby: "ab" * 3
来源：http://bik.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jpf.nanxinkj.top

[E03] 截取子串
来源：http://acf.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lcv.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fbi.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xqb.xinyue.icu

TS:   s.slice(1, 4)
来源：http://gtb.hywenlv.cn

Java: s.substring(1, 4)
来源：http://tnq.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ctc.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ohd.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://onl.zhoulong.xyz

[E04] 查找子串位置
来源：http://ktv.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://qos.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://zlh.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hpo.zhengqikj.top

TS:   s.indexOf("x")
来源：http://dhc.gotoacloud.top

Java: s.indexOf("x")
来源：http://kaq.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://knw.ydjk.org.cn

Ruby: s.index("x")
来源：http://nvm.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://sid.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xws.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sxf.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://off.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sgj.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uml.yanxiufei.cn


<!-- 参考信息 -->