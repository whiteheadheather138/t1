代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qrg.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nht.uphjek.com

Java: // 无解构
来源：http://ufz.hammf.cn

Go:   // 无解构
来源：http://ebn.nwbrower.top

Ruby: a, b = pair
来源：http://mqy.uphjek.com

C#:   var (a, b) = pair;
来源：http://cry.pycfn.com

[C16] 函数 / 方法重载
来源：http://eke.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pjm.jlsjyb.cn

PHP:  // 无重载
来源：http://hpu.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ooz.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://slt.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://jhk.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://chz.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://gjv.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uaq.hfpthk.cn

================================================================================
来源：http://hih.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://jwp.jianghu66.top

================================================================================
来源：http://ldg.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://hjy.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ali.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://voj.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ils.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yoc.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lfw.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://hvu.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://afi.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jfz.jinqigufen.top

[D02] 追加元素到末尾
来源：http://ohj.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nuh.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zdh.xziqi.cn

JS:   arr.push(4);
来源：http://ror.xuanzx.com

TS:   arr.push(4);
来源：http://cdf.hywenlv.cn

Java: list.add(4);
来源：http://uki.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://nis.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://rwi.andypj.xyz

C#:   list.Add(4);
来源：http://jis.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://qnl.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://uty.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xpg.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mhj.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://rdz.aizwys.cn

Java: list.add(0, 0);
来源：http://lzz.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://leh.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://abj.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://qpl.havefunace.top

[D04] 删除元素
来源：http://fqf.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://flo.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://phu.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ell.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://cmx.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sap.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jww.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iet.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btl.bbcook.cn

[D05] 访问与修改元素
来源：http://ilj.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rct.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yvt.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jfp.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://gcv.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://nua.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://rgo.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uty.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xzx.jyoumei.cn

[D06] 数组长度
来源：http://xym.zdqjudy.top

Py:   len(arr)
来源：http://oty.quarkkingdee.top

PHP:  count($arr);
来源：http://pnm.yangfankeji.com

JS:   arr.length
来源：http://eox.sjlbkw.cn

TS:   arr.length
来源：http://wfb.52xcode.cn

Java: list.size();
来源：http://die.chenlongwang.top

Go:   len(arr)
来源：http://gmi.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://tyk.yonumen.top

C#:   list.Count;
来源：http://gud.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://mef.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ldk.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jia.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://ene.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://bvw.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://yts.shuidangran.top

Go:   arr[1:4]
来源：http://vwz.yj202588.top

Ruby: arr[1, 3]
来源：http://cfn.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://drm.svipenyu.cn

[D08] 合并两个数组
来源：http://frv.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://niv.yongpay.top

PHP:  array_merge($a, $b);
来源：http://eei.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://afd.xinyue.icu

TS:   [...a, ...b];
来源：http://yzh.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gim.vehdjk.com

Go:   append(a, b...)
来源：http://irp.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://raa.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://eon.9152youxi.cn

[D09] 排序（升序）
来源：http://egg.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://kri.mhx1999.top

PHP:  sort($arr);
来源：http://vus.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tnx.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://yrq.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hoo.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nxf.yueranfly.top

Ruby: arr.sort
来源：http://kqo.iojbl.cn

C#:   list.Sort();
来源：http://nhr.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bso.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yev.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://erl.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qed.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eok.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://znv.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbc.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eua.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tak.xziqi.cn

[D11] 反转数组
来源：http://vpo.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pjv.hnqzz.top

PHP:  array_reverse($arr);
来源：http://gmd.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mfk.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://gpp.tarul.cn

Java: Collections.reverse(list);
来源：http://slw.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://vbs.nanxinkj.top

Ruby: arr.reverse
来源：http://kig.fengsongda.top

C#:   list.Reverse();
来源：http://rxs.redwolf501.top

[D12] 查找元素下标
来源：http://kak.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://opp.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lhs.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yua.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fwa.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qmr.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://hfl.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://mhi.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://udu.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://mjs.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qiu.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzx.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://zhq.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://qav.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kxu.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lee.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://nai.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://foq.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://tji.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jgy.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yuw.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://zur.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://zcd.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kif.hcnkem.com

Go:   // 手写循环
来源：http://uaq.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://gsf.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yzi.cheryme.top

[D15] 去重
来源：http://kpo.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qzd.sweek.top

PHP:  array_unique($arr);
来源：http://glf.316326.xyz

JS:   [...new Set(arr)]
来源：http://vox.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://hwd.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvy.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://fgw.sjlbkw.cn

Ruby: arr.uniq
来源：http://lnw.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://nnv.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://rhg.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mtr.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ndk.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zai.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxb.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pke.shuidangran.top

Go:   // 手写循环累加
来源：http://wfk.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pag.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://qut.hnxiangtu.top

[D17] 最大值与最小值
来源：http://dxt.birdmap.top

Py:   max(arr);  min(arr)
来源：http://tnc.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://mlv.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nsg.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://bdw.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://inj.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://suz.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://dvi.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://ixw.cashguo.top

[D18] 扁平化嵌套数组
来源：http://uhz.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yjr.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://rgo.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wej.ivvv.top

TS:   nested.flat();
来源：http://izg.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vgc.sufxvd.cn

Go:   // 手写双层循环
来源：http://egq.yj20258.top

Ruby: nested.flatten
来源：http://fij.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://pej.c1oappe.top

[D19] 按字段分组
来源：http://fws.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rgu.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jfj.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rrt.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ywq.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pro.316326.xyz

Go:   // 手写 map[string][]T
来源：http://eom.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://efp.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kry.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://atz.sxryk.cn

Py:   Counter(arr)
来源：http://qzd.aizwys.cn

PHP:  array_count_values($arr);
来源：http://eng.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xcm.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fhm.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iux.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://hxe.zhoulong.xyz

Ruby: arr.tally
来源：http://bsm.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sym.c1oappe.top

[D21] 判断是否包含某元素
来源：http://veu.cashguo.top

Py:   x in arr
来源：http://rbr.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://tia.yangfankeji.com

JS:   arr.includes(x)
来源：http://pba.nwbrower.top

TS:   arr.includes(x)
来源：http://wnn.zhiwuduotai.top

Java: list.contains(x)
来源：http://phe.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://dbd.cqqwz.cn

Ruby: arr.include?(x)
来源：http://kyr.guannengcc.top

C#:   list.Contains(x)
来源：http://lcd.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://nkk.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vdo.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kon.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hzn.yj20258.top

TS:   [...arr];
来源：http://hgc.ivvv.top

Java: new ArrayList<>(list);
来源：http://tft.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qwe.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://cjj.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://euw.yongpay.top

[D23] reduce 累积计算
来源：http://ivu.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qla.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hjk.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmi.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjb.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wqe.fengsongda.top

Go:   // 手写循环
来源：http://zgl.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xjp.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gmq.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://cne.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mgd.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://umu.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mcv.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ypm.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xrb.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://smj.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ewy.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ccv.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://pya.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vpf.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bgt.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eoa.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rjb.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://brm.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gqa.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dwt.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lyp.wangshuangyany.cn

[D26] 数组转字符串
来源：http://jvx.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://egd.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://uua.uphjek.com

JS:   arr.join(", ")
来源：http://kvm.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://kcs.epnwcf.com

Java: String.join(", ", list)
来源：http://tle.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://wbz.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://mam.hesvh.cn

C#:   string.Join(", ", list)
来源：http://xop.havefunace.top

================================================================================
来源：http://iaa.hammf.cn

E. 字符串处理
来源：http://dhp.jinyuanbaomall.cn

================================================================================
来源：http://jhb.chenjidiqi.icu

[E01] 拼接字符串
来源：http://ihn.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vwk.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wgh.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kox.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqe.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fkw.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gzb.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfk.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dah.birdmap.top

[E02] 重复字符串
来源：http://twi.jiagoushi.top

Py:   "ab" * 3
来源：http://wgi.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://pvi.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://hmj.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://ynw.meibo888.top

Java: "ab".repeat(3)
来源：http://wfv.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://dye.9152youxi.cn

Ruby: "ab" * 3
来源：http://cep.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rpa.shuidangran.top

[E03] 截取子串
来源：http://qvf.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sak.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rnj.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://frq.jianghu66.top

TS:   s.slice(1, 4)
来源：http://dev.havefunace.top

Java: s.substring(1, 4)
来源：http://wjb.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jvt.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://mnm.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://ycv.jiagoushi.top

[E04] 查找子串位置
来源：http://sow.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://wlo.guannengcc.top

PHP:  strpos($s, "x");
来源：http://yib.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wwj.zhengqikj.top

TS:   s.indexOf("x")
来源：http://kbr.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://waq.yonumen.top

Go:   strings.Index(s, "x")
来源：http://tzj.guowangkeji.top

Ruby: s.index("x")
来源：http://cax.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://htu.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://xju.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pad.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gdb.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://paz.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://nkq.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fvg.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qnz.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://alv.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myv.aizwys.cn


<!-- 参考信息 -->