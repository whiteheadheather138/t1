代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fwd.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gie.yuanzhike.top

Java: // 无解构
来源：http://evf.shuidangran.top

Go:   // 无解构
来源：http://qgq.nanxuanxn.top

Ruby: a, b = pair
来源：http://glk.daxiang520.top

C#:   var (a, b) = pair;
来源：http://dgt.cucudq.cn

[C16] 函数 / 方法重载
来源：http://jmi.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ess.wangdashe.top

PHP:  // 无重载
来源：http://usv.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lgg.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://ntn.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zfy.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://brz.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://ycz.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pgd.tarul.cn

================================================================================
来源：http://lhl.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://swr.epnwcf.com

================================================================================
来源：http://cbq.meibo888.top

[D01] 创建数组 / 列表
来源：http://uqo.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kww.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://srm.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rqn.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nju.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qye.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://gfr.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://zii.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kbj.316326.xyz

[D02] 追加元素到末尾
来源：http://rgc.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgx.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lhx.cheryme.top

JS:   arr.push(4);
来源：http://wil.c1oappe.top

TS:   arr.push(4);
来源：http://owo.hcnkem.com

Java: list.add(4);
来源：http://yhd.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://awu.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://gnj.hongshengwenyu.top

C#:   list.Add(4);
来源：http://ghp.yj20258888.top

[D03] 在指定位置插入元素
来源：http://nqu.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://nmx.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hkj.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zep.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://hcr.jinqigufen.top

Java: list.add(0, 0);
来源：http://vsn.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wil.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://weo.yongpay.top

C#:   list.Insert(0, 0);
来源：http://kwx.kuanghao11.cn

[D04] 删除元素
来源：http://plj.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fok.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://har.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqq.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://xkk.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://agt.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ovi.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsr.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vyt.ivvv.top

[D05] 访问与修改元素
来源：http://hvo.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fpd.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://thu.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kps.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://xmz.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://hyj.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://jhl.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eqv.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fnk.shanyushiyangkeji.top

[D06] 数组长度
来源：http://zgw.nwbrower.top

Py:   len(arr)
来源：http://iyt.xinyue.icu

PHP:  count($arr);
来源：http://gtr.guannengcc.top

JS:   arr.length
来源：http://sym.uphjek.com

TS:   arr.length
来源：http://rvs.zdqjudy.top

Java: list.size();
来源：http://rxx.316326.xyz

Go:   len(arr)
来源：http://ahq.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://whk.jyoumei.cn

C#:   list.Count;
来源：http://gym.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://boy.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qno.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://enu.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://nqu.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://rob.jianghu66.top

Java: list.subList(1, 4);
来源：http://fdh.fzhhl.top

Go:   arr[1:4]
来源：http://bvs.havefunace.top

Ruby: arr[1, 3]
来源：http://dkm.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://yie.snrcjt.cn

[D08] 合并两个数组
来源：http://iig.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://qxm.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://bpy.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://khs.quarkkingdee.top

TS:   [...a, ...b];
来源：http://imq.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ymt.guannengcc.top

Go:   append(a, b...)
来源：http://pqk.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://irf.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://aad.yj20258.top

[D09] 排序（升序）
来源：http://fhl.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ljk.sjlbkw.cn

PHP:  sort($arr);
来源：http://egp.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nmo.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iaz.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fxo.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nmf.epnwcf.com

Ruby: arr.sort
来源：http://ljb.yuanzhike.top

C#:   list.Sort();
来源：http://gxe.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxf.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ctl.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgk.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gyx.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zql.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ktj.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gzz.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jba.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hub.cashguo.top

[D11] 反转数组
来源：http://fjq.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xfu.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://frq.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ghx.guannengcc.top

TS:   [...arr].reverse();
来源：http://oum.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://hvm.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://scl.hfpthk.cn

Ruby: arr.reverse
来源：http://pst.guannengcc.top

C#:   list.Reverse();
来源：http://dlg.jyoumei.cn

[D12] 查找元素下标
来源：http://zva.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://uly.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqe.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zka.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tlb.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hgk.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://qax.sjlbkw.cn

Ruby: arr.index(x)
来源：http://med.yj20258888.top

C#:   list.IndexOf(x);
来源：http://zsz.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://bfz.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oao.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gww.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://hpu.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://lge.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tli.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xsy.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://mve.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wxn.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://mdw.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://box.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lnu.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://cuj.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://rfw.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yrv.yvedp.cn

Go:   // 手写循环
来源：http://cva.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://izn.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://muc.gogol.net.cn

[D15] 去重
来源：http://qwf.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oae.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://xvu.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://bzp.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://gsx.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qet.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fhy.uphjek.com

Ruby: arr.uniq
来源：http://jpa.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://tzx.tianlin.xyz

[D16] 求和与平均值
来源：http://bof.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mtu.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ber.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://leo.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eyf.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lew.zhengqikj.top

Go:   // 手写循环累加
来源：http://aks.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wii.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://oon.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://csr.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://rab.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://lix.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wzh.chenzaomai.com

TS:   Math.max(...arr);
来源：http://pkl.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lgo.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://foo.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://wum.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://lzo.havefunace.top

[D18] 扁平化嵌套数组
来源：http://hbw.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rxi.cashguo.top

PHP:  array_merge(...$nested);
来源：http://xiz.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hwc.ctjpmb.com

TS:   nested.flat();
来源：http://lgr.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zkd.havefunace.top

Go:   // 手写双层循环
来源：http://hmg.gotoacloud.top

Ruby: nested.flatten
来源：http://kzh.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsu.yvedp.cn

[D19] 按字段分组
来源：http://olu.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mph.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dae.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://agw.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zom.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tmo.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://jqe.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bng.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xfx.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://sxz.yueranfly.top

Py:   Counter(arr)
来源：http://yxd.xuanzx.com

PHP:  array_count_values($arr);
来源：http://ctn.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://igo.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eaw.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zqi.andypj.xyz

Go:   // 手写 map[T]int
来源：http://jbh.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://qvf.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fmx.yonumen.top

[D21] 判断是否包含某元素
来源：http://auy.wangdashe.top

Py:   x in arr
来源：http://dwc.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://qmf.smart0.xyz

JS:   arr.includes(x)
来源：http://ezr.fengsongda.top

TS:   arr.includes(x)
来源：http://myg.gotoacloud.top

Java: list.contains(x)
来源：http://lbp.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://kqt.jiagoushi.top

Ruby: arr.include?(x)
来源：http://vyk.316326.xyz

C#:   list.Contains(x)
来源：http://txw.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://pkq.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bwc.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://khd.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eoq.snrcjt.cn

TS:   [...arr];
来源：http://ywq.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://mbo.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://jlr.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://xcf.vqdsnc.cn

C#:   new List<int>(list);
来源：http://uvc.gotoacloud.top

[D23] reduce 累积计算
来源：http://szd.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wzi.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ivh.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qpo.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wub.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://miz.xziqi.cn

Go:   // 手写循环
来源：http://qme.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfi.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qsb.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://qfe.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yet.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://umg.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwg.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oig.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://non.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ysq.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izw.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://htu.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://yhf.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fmi.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vju.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://grk.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vkg.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zun.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fzg.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lmf.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xcr.hnxiangtu.top

[D26] 数组转字符串
来源：http://yxj.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://fhd.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://ujl.ydzc1.top

JS:   arr.join(", ")
来源：http://loq.zhongyouzk.top

TS:   arr.join(", ")
来源：http://gxo.kuanghao11.cn

Java: String.join(", ", list)
来源：http://kuo.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://oww.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://uea.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://lwn.yvedp.cn

================================================================================
来源：http://sln.jianghu66.top

E. 字符串处理
来源：http://tti.snrcjt.cn

================================================================================
来源：http://dqy.yj202588.top

[E01] 拼接字符串
来源：http://whw.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://svu.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bak.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://twf.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bre.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dma.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tod.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wwb.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzs.gzhubu.top

[E02] 重复字符串
来源：http://ybe.yanxiufei.cn

Py:   "ab" * 3
来源：http://rco.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://mkx.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://ukb.hnqzz.top

TS:   "ab".repeat(3)
来源：http://xtq.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://gwz.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://kep.cashguo.top

Ruby: "ab" * 3
来源：http://wvj.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pzc.snrcjt.cn

[E03] 截取子串
来源：http://rlr.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oaz.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ivv.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tav.xziqi.cn

TS:   s.slice(1, 4)
来源：http://cvq.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://gjq.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kph.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://zgk.yj202588.top

C#:   s.Substring(1, 3)
来源：http://wrt.yongpay.top

[E04] 查找子串位置
来源：http://kow.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://aay.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://exz.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fjo.sxryk.cn

TS:   s.indexOf("x")
来源：http://ojm.gogol.net.cn

Java: s.indexOf("x")
来源：http://omz.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://xbd.nanxinkj.top

Ruby: s.index("x")
来源：http://yfg.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://gsh.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tln.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://can.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xvx.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sun.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://soj.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bqi.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://glj.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ocq.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fqj.0kj1m.cn


<!-- 参考信息 -->