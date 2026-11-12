代发 wailian999

Ruby: a, b = pair
来源：http://xcg.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://aej.yvedp.cn

[C16] 函数 / 方法重载
来源：http://zue.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fmv.fanxiaobao.xyz

PHP:  // 无重载
来源：http://cqx.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqv.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://byy.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zdq.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://zcp.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://mal.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wpb.snrcjt.cn

================================================================================
来源：http://ehp.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://wlc.wangdashe.top

================================================================================
来源：http://ouy.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://dzl.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://upn.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmo.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lzm.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vlj.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cfn.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://xqj.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://aom.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vsh.redwolf501.top

[D02] 追加元素到末尾
来源：http://atj.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aku.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://okv.fktsv.cn

JS:   arr.push(4);
来源：http://sbw.hongshengwenyu.top

TS:   arr.push(4);
来源：http://yqx.shangyingyoupin.top

Java: list.add(4);
来源：http://elt.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://yuq.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://vrj.jianghu66.top

C#:   list.Add(4);
来源：http://mzu.uphjek.com

[D03] 在指定位置插入元素
来源：http://ubf.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://owa.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qtg.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pyi.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://pza.ydzc1.top

Java: list.add(0, 0);
来源：http://pfb.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://onx.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cpp.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://nnp.chenzaomai.com

[D04] 删除元素
来源：http://ndb.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ttq.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dsv.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nff.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://rpp.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dbp.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://slp.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qht.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cod.haohaochexian.top

[D05] 访问与修改元素
来源：http://vdy.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mun.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ajp.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wlr.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://scu.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://cwu.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://adb.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://itj.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zoc.yj202588.top

[D06] 数组长度
来源：http://cfx.xuetiantiany.cn

Py:   len(arr)
来源：http://ypv.fzhhl.top

PHP:  count($arr);
来源：http://ttv.gaohongyu789.top

JS:   arr.length
来源：http://jhb.gotoacloud.top

TS:   arr.length
来源：http://vhi.iojbl.cn

Java: list.size();
来源：http://kcd.epnwcf.com

Go:   len(arr)
来源：http://rte.guannengcc.top

Ruby: arr.length; arr.size
来源：http://tur.ydjk.org.cn

C#:   list.Count;
来源：http://pgo.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://bhx.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iip.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://szh.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://nit.cdnleiting.top

TS:   arr.slice(1, 4);
来源：http://mzz.yuanzhike.top

Java: list.subList(1, 4);
来源：http://ftb.snrcjt.cn

Go:   arr[1:4]
来源：http://pny.epnwcf.com

Ruby: arr[1, 3]
来源：http://pxj.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://lts.jqgfzy.top

[D08] 合并两个数组
来源：http://qbd.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://kui.cheryme.top

PHP:  array_merge($a, $b);
来源：http://wvi.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iuo.ctjpmb.com

TS:   [...a, ...b];
来源：http://dof.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nms.sysykeji.top

Go:   append(a, b...)
来源：http://eof.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://jan.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://rut.vehdjk.com

[D09] 排序（升序）
来源：http://aot.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://jdr.xuetiantiany.cn

PHP:  sort($arr);
来源：http://kzm.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xrd.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hfu.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://igc.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xpb.jiagoushi.top

Ruby: arr.sort
来源：http://jay.hfpthk.cn

C#:   list.Sort();
来源：http://inm.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tox.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qzp.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cub.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://epe.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ljn.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://prx.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bzv.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://quo.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zyv.zhongyouzk.top

[D11] 反转数组
来源：http://wyq.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://dxu.fzhhl.top

PHP:  array_reverse($arr);
来源：http://nhs.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lll.jinqigufen.top

TS:   [...arr].reverse();
来源：http://asj.guannengcc.top

Java: Collections.reverse(list);
来源：http://cul.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://eua.sjlbkw.cn

Ruby: arr.reverse
来源：http://rex.haohaochexian.top

C#:   list.Reverse();
来源：http://qgy.zhongyouzk.top

[D12] 查找元素下标
来源：http://xby.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://otw.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yjr.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqa.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://erw.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rvs.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://ayn.daria6918.cn

Ruby: arr.index(x)
来源：http://xls.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://mfh.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://exk.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sob.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ndl.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://ijc.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://qcf.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cxk.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bzw.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://chh.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bbk.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://cyk.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rgk.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xjh.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://wbq.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://vqm.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pls.jyoumei.cn

Go:   // 手写循环
来源：http://dou.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://zgq.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kor.yuanzhike.top

[D15] 去重
来源：http://ccu.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uug.gogol.net.cn

PHP:  array_unique($arr);
来源：http://pmv.yj202588.top

JS:   [...new Set(arr)]
来源：http://mff.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://iri.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tjk.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://lqe.vqdsnc.cn

Ruby: arr.uniq
来源：http://eyv.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://yvj.vqdsnc.cn

[D16] 求和与平均值
来源：http://dyz.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://evp.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ogw.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://grf.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bfg.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tce.zhoulong.xyz

Go:   // 手写循环累加
来源：http://zzu.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bwk.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://dgq.epnwcf.com

[D17] 最大值与最小值
来源：http://dfv.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://mfk.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://dix.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ahk.mhx1999.top

TS:   Math.max(...arr);
来源：http://zts.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sbq.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vfr.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://zyj.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://iyb.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://pvs.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mcf.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://ajh.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xfx.chenzaomai.com

TS:   nested.flat();
来源：http://wut.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://isp.aizwys.cn

Go:   // 手写双层循环
来源：http://lcl.zhijiandao.cn

Ruby: nested.flatten
来源：http://nev.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jrs.aibaodan.cn

[D19] 按字段分组
来源：http://ujj.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://swu.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wus.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yxi.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fsu.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zoa.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://tmb.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jgl.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://svd.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://ygl.zycfv.cn

Py:   Counter(arr)
来源：http://gbe.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://pcl.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qyh.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hls.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gue.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://rqm.xinyue.icu

Ruby: arr.tally
来源：http://vib.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mtx.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://mcg.guannengcc.top

Py:   x in arr
来源：http://bdh.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://ykk.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://sin.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://hjt.yj20258.top

Java: list.contains(x)
来源：http://vir.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://vsf.yangfankeji.com

Ruby: arr.include?(x)
来源：http://axf.yj20258888.top

C#:   list.Contains(x)
来源：http://xkt.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://gzs.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eoq.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fwq.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qxp.jianghu66.top

TS:   [...arr];
来源：http://zpb.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://kcw.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://koa.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://cwf.yj20258.top

C#:   new List<int>(list);
来源：http://yyr.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://cbv.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vdu.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qmn.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfk.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhr.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://cev.nwbrower.top

Go:   // 手写循环
来源：http://yej.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://drz.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wrd.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://ypo.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hup.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdx.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpc.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://brh.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vex.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqc.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gqt.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ojy.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://qil.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iuv.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jpf.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tni.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mtr.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nqx.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fmh.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://klc.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bij.cashguo.top

[D26] 数组转字符串
来源：http://lpq.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://cwl.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://biy.svipenyu.cn

JS:   arr.join(", ")
来源：http://nhr.havefunace.top

TS:   arr.join(", ")
来源：http://okb.andypj.xyz

Java: String.join(", ", list)
来源：http://zjr.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://hnf.ctjpmb.com

Ruby: arr.join(", ")
来源：http://bqi.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://ydx.c1oappe.top

================================================================================
来源：http://fzx.ppjwa.cn

E. 字符串处理
来源：http://weo.yj20258.top

================================================================================
来源：http://yno.xuanzx.com

[E01] 拼接字符串
来源：http://ptk.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nwa.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gpk.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://owe.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mvv.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ote.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gpf.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dyu.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qpj.dashuyun.cn

[E02] 重复字符串
来源：http://fpv.hcnkem.com

Py:   "ab" * 3
来源：http://rlh.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://nmt.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://qps.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://rlw.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://wjy.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://wvz.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://tos.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dmn.jlsjyb.cn

[E03] 截取子串
来源：http://wkd.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://olx.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qat.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqi.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://fhe.ppjwa.cn

Java: s.substring(1, 4)
来源：http://phe.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hvx.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://mwj.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://sqp.fengsongda.top

[E04] 查找子串位置
来源：http://bft.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://sap.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://jva.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ark.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://kkp.yj202588.top

Java: s.indexOf("x")
来源：http://obj.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://xei.zhiwuduotai.top

Ruby: s.index("x")
来源：http://eoq.smart0.xyz

C#:   s.IndexOf("x")
来源：http://abz.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgz.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zzu.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uvg.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvr.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://irw.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zqm.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dka.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://omh.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgl.guowangkeji.top

[E06] 替换子串
来源：http://xts.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jmq.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://mgd.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wwn.zhongyouzk.top


<!-- 参考信息 -->