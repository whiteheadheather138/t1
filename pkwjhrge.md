代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://lin.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://itd.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbw.mhx1999.top

================================================================================
来源：http://nnu.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://bqc.xylfe.cn

================================================================================
来源：http://jsp.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://tvr.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hqw.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bph.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eyf.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fat.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://erw.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jea.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://cae.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ska.ppjwa.cn

[D02] 追加元素到末尾
来源：http://ttf.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://esw.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jkn.hfpthk.cn

JS:   arr.push(4);
来源：http://xsk.wangdashe.top

TS:   arr.push(4);
来源：http://wcb.haohaochexian.top

Java: list.add(4);
来源：http://yhm.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://qxo.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://ilx.meibo888.top

C#:   list.Add(4);
来源：http://kye.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://gax.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://aye.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://coj.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zqe.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://ddu.cdnleiting.top

Java: list.add(0, 0);
来源：http://scf.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uet.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kjg.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://bvz.xuanzx.com

[D04] 删除元素
来源：http://vfg.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tza.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aod.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ghu.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://wru.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fcs.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dxs.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zxb.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wgg.dashuyun.cn

[D05] 访问与修改元素
来源：http://odt.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ald.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://syi.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rqn.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://mwx.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://oyw.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://klg.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://glz.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gjr.hesvh.cn

[D06] 数组长度
来源：http://cob.9152youxi.cn

Py:   len(arr)
来源：http://uyv.xziqi.cn

PHP:  count($arr);
来源：http://iok.sxryk.cn

JS:   arr.length
来源：http://vup.snrcjt.cn

TS:   arr.length
来源：http://yld.xuanzx.com

Java: list.size();
来源：http://vzd.ydzc1.top

Go:   len(arr)
来源：http://upj.aizwys.cn

Ruby: arr.length; arr.size
来源：http://kko.jianghu66.top

C#:   list.Count;
来源：http://dgb.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://fza.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ggv.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://hrz.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://ofb.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://xoe.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://nes.pengpengdd.cyou

Go:   arr[1:4]
来源：http://nkq.yj202588.top

Ruby: arr[1, 3]
来源：http://xam.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://okb.cdnleiting.top

[D08] 合并两个数组
来源：http://kzz.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://szr.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://luc.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fmb.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://ydv.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrm.yangfankeji.com

Go:   append(a, b...)
来源：http://sxg.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://vih.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://nzr.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://epx.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://hev.fzhhl.top

PHP:  sort($arr);
来源：http://osr.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aph.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rde.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lix.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bxc.pycfn.com

Ruby: arr.sort
来源：http://utj.epnwcf.com

C#:   list.Sort();
来源：http://psv.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wdv.chenzaomai.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wgn.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lid.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hff.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ywk.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dmw.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wet.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://twe.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bwt.jiagoushi.top

[D11] 反转数组
来源：http://ogn.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://bba.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://van.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nzw.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://iwq.yuxming.cn

Java: Collections.reverse(list);
来源：http://ffd.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://ijf.yvedp.cn

Ruby: arr.reverse
来源：http://fbg.epnwcf.com

C#:   list.Reverse();
来源：http://cbw.quarkkingdee.top

[D12] 查找元素下标
来源：http://dav.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://ckn.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zcx.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mnz.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://urc.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vkj.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://xsq.52xcode.cn

Ruby: arr.index(x)
来源：http://rmt.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://lll.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://cvi.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://umu.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rpw.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://mzr.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://odw.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mee.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fdy.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dqj.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://owi.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://eoi.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xld.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://was.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://eix.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://gcy.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kek.xuanzx.com

Go:   // 手写循环
来源：http://yxl.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://wto.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://awm.9152youxi.cn

[D15] 去重
来源：http://jvy.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lxe.ctjpmb.com

PHP:  array_unique($arr);
来源：http://ozf.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://nxw.yj202588.top

TS:   [...new Set(arr)]
来源：http://vmx.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xoy.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mtl.epnwcf.com

Ruby: arr.uniq
来源：http://npn.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://jxw.sufxvd.cn

[D16] 求和与平均值
来源：http://lmd.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dqi.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://muq.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzn.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzy.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vwg.ctjpmb.com

Go:   // 手写循环累加
来源：http://cof.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cso.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://lvp.sweek.top

[D17] 最大值与最小值
来源：http://rpo.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://abe.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://pay.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oyp.birdmap.top

TS:   Math.max(...arr);
来源：http://scz.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wcw.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hge.yj20258.top

Ruby: arr.max;  arr.min
来源：http://yfw.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://mlb.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://jcj.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bsq.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://fau.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ofn.hnqzz.top

TS:   nested.flat();
来源：http://rrl.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qjl.pycfn.com

Go:   // 手写双层循环
来源：http://czy.cdnleiting.top

Ruby: nested.flatten
来源：http://hjk.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://cem.cqqwz.cn

[D19] 按字段分组
来源：http://txs.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wea.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://puf.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpe.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ppm.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pwg.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://oyj.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xew.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qco.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://vdt.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://spe.bjfxy.top

PHP:  array_count_values($arr);
来源：http://sza.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwj.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xha.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gwc.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://vzc.sysykeji.top

Ruby: arr.tally
来源：http://tvd.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uir.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://uya.xylfe.cn

Py:   x in arr
来源：http://usb.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://nsl.ydzc1.top

JS:   arr.includes(x)
来源：http://uno.jyoumei.cn

TS:   arr.includes(x)
来源：http://ufq.ydzc1.top

Java: list.contains(x)
来源：http://hvd.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://jql.dianchejie.cn

Ruby: arr.include?(x)
来源：http://vrm.hywenlv.cn

C#:   list.Contains(x)
来源：http://wdi.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://gxa.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://imk.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nne.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mrv.yuanzhike.top

TS:   [...arr];
来源：http://enz.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://gae.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://dwa.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://xfh.ybcxt.top

C#:   new List<int>(list);
来源：http://eem.aibaodan.cn

[D23] reduce 累积计算
来源：http://qdh.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fex.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zxm.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvs.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zwa.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fgd.nanxinkj.top

Go:   // 手写循环
来源：http://pjx.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lok.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qie.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://nru.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mza.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zli.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hjd.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lmr.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://smz.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ngz.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gjd.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://thh.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://qax.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ehf.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://czg.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pup.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://itf.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vpk.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hpr.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xcc.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vma.9152youxi.cn

[D26] 数组转字符串
来源：http://njc.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://nfa.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://cdu.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://mlo.fengsongda.top

TS:   arr.join(", ")
来源：http://odm.jinqigufen.top

Java: String.join(", ", list)
来源：http://huy.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://iyp.mhx1999.top

Ruby: arr.join(", ")
来源：http://woh.ywan-chungtsiang.top

C#:   string.Join(", ", list)
来源：http://kjb.fengsongda.top

================================================================================
来源：http://ysx.epnwcf.com

E. 字符串处理
来源：http://wzw.shuidangran.top

================================================================================
来源：http://oid.mhx1999.top

[E01] 拼接字符串
来源：http://cjk.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ldr.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kcp.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpz.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnw.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hav.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://paz.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ulh.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tib.shzxlz.cn

[E02] 重复字符串
来源：http://chu.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://pih.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://qfn.xylfe.cn

JS:   "ab".repeat(3)
来源：http://nqe.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://rvj.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://ula.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://ilo.dianchejie.cn

Ruby: "ab" * 3
来源：http://dle.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ccu.hnxiangtu.top

[E03] 截取子串
来源：http://bss.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xfm.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jyt.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sut.tian-w.cn

TS:   s.slice(1, 4)
来源：http://uca.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://flo.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hcf.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jtw.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://ndx.0kj1m.cn

[E04] 查找子串位置
来源：http://ysc.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://isb.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://zaf.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://czv.smart0.xyz

TS:   s.indexOf("x")
来源：http://ejg.gogol.net.cn

Java: s.indexOf("x")
来源：http://zbg.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://pgm.bbcook.cn

Ruby: s.index("x")
来源：http://eny.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://ckx.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mri.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://knd.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vzs.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgl.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bio.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ine.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://knf.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://riq.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xcx.nanxinkj.top

[E06] 替换子串
来源：http://qrx.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vul.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://nal.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://paa.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://zlh.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdy.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vwz.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lyo.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://qgt.jinqigufen.top

[E07] 按分隔符拆分
来源：http://ztz.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tfn.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://utn.epnwcf.com


<!-- 参考信息 -->