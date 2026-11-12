代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rqa.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ipc.yuxming.cn

Java: // 无解构
来源：http://cip.shzxlz.cn

Go:   // 无解构
来源：http://xik.gogol.net.cn

Ruby: a, b = pair
来源：http://mhx.xylfe.cn

C#:   var (a, b) = pair;
来源：http://mek.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://ged.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zsk.chenlongwang.top

PHP:  // 无重载
来源：http://ess.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tfh.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://eje.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ydu.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://ugr.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://qtz.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://quq.yanxiufei.cn

================================================================================
来源：http://kks.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://omf.uphjek.com

================================================================================
来源：http://jdn.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://ifa.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://alo.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wbs.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mvl.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rnv.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sax.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://gwm.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://ees.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xas.fengsongda.top

[D02] 追加元素到末尾
来源：http://cin.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tfr.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zrm.chenlongwang.top

JS:   arr.push(4);
来源：http://daz.dianchejie.cn

TS:   arr.push(4);
来源：http://csp.meibo888.top

Java: list.add(4);
来源：http://ssg.tarul.cn

Go:   arr = append(arr, 4)
来源：http://xct.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://occ.ppjwa.cn

C#:   list.Add(4);
来源：http://jjr.daxiang520.top

[D03] 在指定位置插入元素
来源：http://ccx.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://zdl.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ndf.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nyz.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://dpr.zhoulong.xyz

Java: list.add(0, 0);
来源：http://crr.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://arf.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qtk.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://omh.meibo888.top

[D04] 删除元素
来源：http://yid.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zsd.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xll.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://peh.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://edq.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yon.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jdz.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjk.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://seq.zdqjudy.top

[D05] 访问与修改元素
来源：http://srl.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mrd.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://syv.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xid.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://mrj.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ohg.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://njy.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fmp.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blb.jqgfzy.top

[D06] 数组长度
来源：http://pha.mhx1999.top

Py:   len(arr)
来源：http://zps.svipenyu.cn

PHP:  count($arr);
来源：http://zxf.jianghu66.top

JS:   arr.length
来源：http://qis.redwolf501.top

TS:   arr.length
来源：http://ajo.vqdsnc.cn

Java: list.size();
来源：http://hlg.yuanzhike.top

Go:   len(arr)
来源：http://ngt.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://fmi.chenlongwang.top

C#:   list.Count;
来源：http://hxw.fktsv.cn

[D07] 切片 / 取子数组
来源：http://dqx.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yhl.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ikk.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://yfn.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://iew.0kj1m.cn

Java: list.subList(1, 4);
来源：http://igq.bjfxy.top

Go:   arr[1:4]
来源：http://oqm.chenlongwang.top

Ruby: arr[1, 3]
来源：http://bwv.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://scf.hesvh.cn

[D08] 合并两个数组
来源：http://clu.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://bro.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://mzm.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://npt.hcnkem.com

TS:   [...a, ...b];
来源：http://gcm.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wnh.yj20258.top

Go:   append(a, b...)
来源：http://qtz.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://rcq.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://mju.c1oappe.top

[D09] 排序（升序）
来源：http://dto.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ymp.cheryme.top

PHP:  sort($arr);
来源：http://dea.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nlu.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lds.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gtg.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ags.ydjk.org.cn

Ruby: arr.sort
来源：http://vnr.jinghuilouyu.cn

C#:   list.Sort();
来源：http://zoc.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://kkv.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cgq.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kdl.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gxn.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://auc.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jlp.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nud.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mso.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://trz.jinqigfzy.top

[D11] 反转数组
来源：http://gax.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://goi.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://owi.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://els.hywenlv.cn

TS:   [...arr].reverse();
来源：http://dsv.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://qie.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://ban.bbcook.cn

Ruby: arr.reverse
来源：http://yex.fengsongda.top

C#:   list.Reverse();
来源：http://atv.chenjidiqi.icu

[D12] 查找元素下标
来源：http://kmp.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://yag.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jpn.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iap.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qua.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ywx.havefunace.top

Go:   slices.Index(arr, x)
来源：http://ckp.cashguo.top

Ruby: arr.index(x)
来源：http://aux.meibo888.top

C#:   list.IndexOf(x);
来源：http://vvq.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://tcw.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfj.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kwp.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://noe.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://qrf.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aoa.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kbi.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://zcv.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://whc.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://vue.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kxx.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jys.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://iqv.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://dxt.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bms.jqgufenzy.top

Go:   // 手写循环
来源：http://iwm.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jyc.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ljf.cheryme.top

[D15] 去重
来源：http://jwn.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ypt.hywenlv.cn

PHP:  array_unique($arr);
来源：http://ygh.cucudq.cn

JS:   [...new Set(arr)]
来源：http://apr.sysykeji.top

TS:   [...new Set(arr)]
来源：http://eir.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tui.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://bqu.sweek.top

Ruby: arr.uniq
来源：http://kpr.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://gbh.xuanzx.com

[D16] 求和与平均值
来源：http://cms.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dbw.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sog.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfy.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gng.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lsm.hnxiangtu.top

Go:   // 手写循环累加
来源：http://uqw.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cad.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://rdx.zhengqikj.top

[D17] 最大值与最小值
来源：http://nni.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://fib.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://tjk.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bup.wangdashe.top

TS:   Math.max(...arr);
来源：http://zvg.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qzm.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dvm.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://zoe.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://ubv.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://xmw.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxi.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://wti.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xtk.zdbjq.cn

TS:   nested.flat();
来源：http://wui.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kme.ctjpmb.com

Go:   // 手写双层循环
来源：http://dgh.jianghu66.top

Ruby: nested.flatten
来源：http://haz.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://owd.jqgfzy.top

[D19] 按字段分组
来源：http://pbi.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pil.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wqz.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bkw.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uil.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pcv.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://qmu.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cuj.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umw.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://hta.zhijiandao.cn

Py:   Counter(arr)
来源：http://oze.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://ymq.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ztk.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rtk.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lvc.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://uyu.dianchejie.cn

Ruby: arr.tally
来源：http://imy.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gxd.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://ozm.ybcxt.top

Py:   x in arr
来源：http://rmu.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://yat.redwolf501.top

JS:   arr.includes(x)
来源：http://epn.zhongyouzk.top

TS:   arr.includes(x)
来源：http://cpm.bbcook.cn

Java: list.contains(x)
来源：http://anu.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://fym.zhixingplan.top

Ruby: arr.include?(x)
来源：http://yfb.nanxuanxn.top

C#:   list.Contains(x)
来源：http://olq.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://njn.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wlv.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ugv.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ygw.zdbjq.cn

TS:   [...arr];
来源：http://hdq.daria6918.cn

Java: new ArrayList<>(list);
来源：http://tre.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://moy.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://ass.hywenlv.cn

C#:   new List<int>(list);
来源：http://veq.sxryk.cn

[D23] reduce 累积计算
来源：http://kdo.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wrx.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lli.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gng.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xyf.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ucu.jyoumei.cn

Go:   // 手写循环
来源：http://jgb.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lnx.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ssp.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://fmu.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://app.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mnm.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jge.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dvv.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fns.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgd.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://abw.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hgg.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://uet.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://spw.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ybi.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kvq.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sfl.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://efd.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://don.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ylv.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rxf.smart0.xyz

[D26] 数组转字符串
来源：http://nit.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://akn.tarul.cn

PHP:  implode(", ", $arr);
来源：http://ptz.pycfn.com

JS:   arr.join(", ")
来源：http://atl.0kj1m.cn

TS:   arr.join(", ")
来源：http://ugs.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://jnk.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://uyy.ydzc1.top

Ruby: arr.join(", ")
来源：http://pzq.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://zpv.jqgfzy.top

================================================================================
来源：http://tws.svipenyu.cn

E. 字符串处理
来源：http://obe.mhx1999.top

================================================================================
来源：http://rwg.yonumen.top

[E01] 拼接字符串
来源：http://eie.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hju.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gki.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfw.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cvt.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rsq.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vjj.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bkj.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yvw.fehbvm.com

[E02] 重复字符串
来源：http://enh.chenlongwang.top

Py:   "ab" * 3
来源：http://hwu.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://shx.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://ees.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://mlh.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://hyt.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://nol.vehdjk.com

Ruby: "ab" * 3
来源：http://pnj.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sdm.316326.xyz

[E03] 截取子串
来源：http://fbh.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kil.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://loj.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://opm.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://edv.wangdashe.top

Java: s.substring(1, 4)
来源：http://yky.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ggr.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://cpl.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://uxl.vehdjk.com

[E04] 查找子串位置
来源：http://tyb.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://ljc.yj20258888.top

PHP:  strpos($s, "x");
来源：http://aya.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://igo.yvedp.cn

TS:   s.indexOf("x")
来源：http://rzq.gzhubu.top

Java: s.indexOf("x")
来源：http://kig.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://idm.tanke756.top

Ruby: s.index("x")
来源：http://gaq.fengsongda.top

C#:   s.IndexOf("x")
来源：http://hjt.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://tcw.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://efk.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ixl.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpf.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kpp.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://frg.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://txs.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eqw.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://niu.vehdjk.com


<!-- 参考信息 -->