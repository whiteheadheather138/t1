代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://doc.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uix.yfazqb.com

Java: // 无解构
来源：http://bwm.ctjpmb.com

Go:   // 无解构
来源：http://pnj.snrcjt.cn

Ruby: a, b = pair
来源：http://gse.yonumen.top

C#:   var (a, b) = pair;
来源：http://lfr.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://klu.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryr.jianghu66.top

PHP:  // 无重载
来源：http://pql.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eha.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://akg.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://etr.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://irv.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://hhg.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://tbo.dashuyun.cn

================================================================================
来源：http://qik.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://bvm.chenlongwang.top

================================================================================
来源：http://dxo.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://iqy.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dki.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ijt.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ojz.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxb.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dwy.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://fia.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://mdz.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vhv.hnqzz.top

[D02] 追加元素到末尾
来源：http://gai.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rsc.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://svz.yuanzhike.top

JS:   arr.push(4);
来源：http://vdm.yvedp.cn

TS:   arr.push(4);
来源：http://ibc.sysykeji.top

Java: list.add(4);
来源：http://iot.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://juw.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://bdx.yj20258.top

C#:   list.Add(4);
来源：http://ncc.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://qfg.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://svn.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvj.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbc.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://mla.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://zvx.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://fau.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gys.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://ugw.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://pej.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qlj.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rbp.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xyu.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://fav.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qqv.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yxq.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hww.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://thg.svipenyu.cn

[D05] 访问与修改元素
来源：http://wlb.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lgh.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jnj.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xrz.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://xoq.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://gpe.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://psd.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aoe.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jmp.mhx1999.top

[D06] 数组长度
来源：http://cnu.jinqigfzy.top

Py:   len(arr)
来源：http://kui.hnqzz.top

PHP:  count($arr);
来源：http://jrg.nwbrower.top

JS:   arr.length
来源：http://fog.bjfxy.top

TS:   arr.length
来源：http://cqw.fanxiaobao.xyz

Java: list.size();
来源：http://wzs.pengpengdd.cyou

Go:   len(arr)
来源：http://mmp.tanke756.top

Ruby: arr.length; arr.size
来源：http://uvk.hesvh.cn

C#:   list.Count;
来源：http://ivd.xziqi.cn

[D07] 切片 / 取子数组
来源：http://boj.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ccl.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tus.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://zht.cheryme.top

TS:   arr.slice(1, 4);
来源：http://iwd.cashguo.top

Java: list.subList(1, 4);
来源：http://uox.epnwcf.com

Go:   arr[1:4]
来源：http://xgg.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://uwj.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://rch.uphjek.com

[D08] 合并两个数组
来源：http://hgh.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://bvy.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://ihx.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rdy.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://jsc.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dmq.vehdjk.com

Go:   append(a, b...)
来源：http://wya.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://jvr.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://zib.sysykeji.top

[D09] 排序（升序）
来源：http://bth.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://agw.cashguo.top

PHP:  sort($arr);
来源：http://hxy.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xeo.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://knm.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zen.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gth.chenlongwang.top

Ruby: arr.sort
来源：http://tab.svipenyu.cn

C#:   list.Sort();
来源：http://ivo.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fnz.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vgw.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bco.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqk.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jve.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejv.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oqq.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nfw.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://frb.hnqzz.top

[D11] 反转数组
来源：http://jcu.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://okf.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://jng.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://moq.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://bfa.cucudq.cn

Java: Collections.reverse(list);
来源：http://ayc.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://sug.ppjwa.cn

Ruby: arr.reverse
来源：http://anb.jqgfzy.top

C#:   list.Reverse();
来源：http://xcl.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://ztz.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://kiz.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lvl.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fju.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osa.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dav.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://hwd.ydjk.org.cn

Ruby: arr.index(x)
来源：http://rnk.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://ibu.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://pur.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dvq.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dpl.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://gmz.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://dfp.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pls.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pfb.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://trd.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pjg.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://fwi.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://abu.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lky.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://win.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://esn.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pyt.epnwcf.com

Go:   // 手写循环
来源：http://msu.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://fzu.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wpt.ppjwa.cn

[D15] 去重
来源：http://wve.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wqf.dashuyun.cn

PHP:  array_unique($arr);
来源：http://vjx.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://mdg.uphjek.com

TS:   [...new Set(arr)]
来源：http://mkb.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ryz.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://ydd.9152youxi.cn

Ruby: arr.uniq
来源：http://ema.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://krb.jqgfzy.top

[D16] 求和与平均值
来源：http://rsl.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdy.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rvw.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejt.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://avq.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zyc.jqgfzy.top

Go:   // 手写循环累加
来源：http://oph.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kec.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://elq.52xcode.cn

[D17] 最大值与最小值
来源：http://bdv.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://wqs.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://koc.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mth.yuanzhike.top

TS:   Math.max(...arr);
来源：http://fxm.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://adf.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ctx.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://kbd.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://alk.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://lkl.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://woq.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://efv.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xak.bjfxy.top

TS:   nested.flat();
来源：http://kde.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ewg.zhijiandao.cn

Go:   // 手写双层循环
来源：http://wlm.jianghu66.top

Ruby: nested.flatten
来源：http://ghv.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xig.guannengcc.top

[D19] 按字段分组
来源：http://hsa.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xjr.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ehx.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mpb.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dmw.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://efj.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://izk.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://thl.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cgd.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://pwl.xylfe.cn

Py:   Counter(arr)
来源：http://zjo.mhx1999.top

PHP:  array_count_values($arr);
来源：http://gcv.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xqk.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xga.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rgt.shuidangran.top

Go:   // 手写 map[T]int
来源：http://fcr.cucudq.cn

Ruby: arr.tally
来源：http://yqk.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xzo.tarul.cn

[D21] 判断是否包含某元素
来源：http://zoj.sufxvd.cn

Py:   x in arr
来源：http://xwi.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://toj.haohaochexian.top

JS:   arr.includes(x)
来源：http://omi.zdbjq.cn

TS:   arr.includes(x)
来源：http://cpt.chenlongwang.top

Java: list.contains(x)
来源：http://qhz.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://jqr.zhengqikj.top

Ruby: arr.include?(x)
来源：http://jnj.hesvh.cn

C#:   list.Contains(x)
来源：http://bzb.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://xiy.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nzp.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rvl.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jiv.tarul.cn

TS:   [...arr];
来源：http://nfj.fktsv.cn

Java: new ArrayList<>(list);
来源：http://etg.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://qzd.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://nnt.zdqjudy.top

C#:   new List<int>(list);
来源：http://rpj.52xcode.cn

[D23] reduce 累积计算
来源：http://fmq.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wsb.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cqh.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bur.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwy.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rad.hnxiangtu.top

Go:   // 手写循环
来源：http://peg.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jis.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bqk.sweek.top

[D24] 字典 / Map 基本操作
来源：http://rkt.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qaa.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jkj.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hoe.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lig.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ici.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://coc.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xvp.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://due.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://pyn.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qec.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pzw.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yen.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dav.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iqx.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zsm.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://siz.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pyo.yanxiufei.cn

[D26] 数组转字符串
来源：http://cxi.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://zns.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://msj.nanxinkj.top

JS:   arr.join(", ")
来源：http://qud.daxiang520.top

TS:   arr.join(", ")
来源：http://ebd.jlsjyb.cn

Java: String.join(", ", list)
来源：http://bkq.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://psh.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://jhw.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://nhz.c1oappe.top

================================================================================
来源：http://bbd.haohaochexian.top

E. 字符串处理
来源：http://ygo.ydjk.org.cn

================================================================================
来源：http://hgt.xylfe.cn

[E01] 拼接字符串
来源：http://skg.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://teq.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uko.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxs.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tnc.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ipz.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ywb.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bxm.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tiu.ehwqpu.com

[E02] 重复字符串
来源：http://coc.redwolf501.top

Py:   "ab" * 3
来源：http://yhb.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://qvs.bjfxy.top

JS:   "ab".repeat(3)
来源：http://orf.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://gcz.ppjwa.cn

Java: "ab".repeat(3)
来源：http://oww.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://oyr.yuxming.cn

Ruby: "ab" * 3
来源：http://qzd.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dtt.ctjpmb.com

[E03] 截取子串
来源：http://dvq.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nte.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xsh.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://njs.xuanzx.com

TS:   s.slice(1, 4)
来源：http://nnr.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://hsv.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oct.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://ruf.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://vao.zdbjq.cn

[E04] 查找子串位置
来源：http://vwb.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://lvj.bjfxy.top

PHP:  strpos($s, "x");
来源：http://ajt.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qim.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://ngs.zdbjq.cn

Java: s.indexOf("x")
来源：http://sbr.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://bbp.hesvh.cn

Ruby: s.index("x")
来源：http://jql.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://pup.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rei.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wlb.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hlk.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mae.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://fmb.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tmw.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tyf.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bmy.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nhh.epnwcf.com


<!-- 参考信息 -->