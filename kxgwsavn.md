代发 wailian999

Ruby: a, b = pair
来源：http://jfo.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://ulo.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://gdo.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mxy.sjlbkw.cn

PHP:  // 无重载
来源：http://pcc.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nda.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://kbm.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lvs.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://pni.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://orn.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qxs.xuetiantiany.cn

================================================================================
来源：http://dtb.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://zny.zhixingplan.top

================================================================================
来源：http://tdv.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://ljq.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uyw.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oeh.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sng.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gyn.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dgd.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://tyx.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://lcz.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pzm.c1oappe.top

[D02] 追加元素到末尾
来源：http://gcx.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tad.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fix.daria6918.cn

JS:   arr.push(4);
来源：http://vnt.zhongyouzk.top

TS:   arr.push(4);
来源：http://nvg.zhijiandao.cn

Java: list.add(4);
来源：http://gro.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://flv.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://mrg.cheryme.top

C#:   list.Add(4);
来源：http://epk.yueranfly.top

[D03] 在指定位置插入元素
来源：http://fyl.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://wol.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mob.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uqw.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://prd.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://dmk.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://exb.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://csk.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://upf.hongshengwenyu.top

[D04] 删除元素
来源：http://yci.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xhm.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hol.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvh.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://rdw.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yrr.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ygd.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kpg.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://crx.chenlongwang.top

[D05] 访问与修改元素
来源：http://yjq.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dre.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://scu.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgz.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ufh.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://lvw.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://yto.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nmi.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bui.tarul.cn

[D06] 数组长度
来源：http://xsw.ydzc1.top

Py:   len(arr)
来源：http://ddq.316326.xyz

PHP:  count($arr);
来源：http://agb.ydzc1.top

JS:   arr.length
来源：http://xug.xingfuxueyuan.xyz

TS:   arr.length
来源：http://ath.birdmap.top

Java: list.size();
来源：http://ncf.guannengcc.top

Go:   len(arr)
来源：http://tqp.sysykeji.top

Ruby: arr.length; arr.size
来源：http://wam.wangdashe.top

C#:   list.Count;
来源：http://eeu.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://nug.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ant.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://plh.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://ijz.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://ssl.meibo888.top

Java: list.subList(1, 4);
来源：http://ttx.hammf.cn

Go:   arr[1:4]
来源：http://yaz.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://zmu.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://gmi.tanke756.top

[D08] 合并两个数组
来源：http://jmq.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://imx.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://sza.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vhd.andypj.xyz

TS:   [...a, ...b];
来源：http://sxh.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://umg.aizwys.cn

Go:   append(a, b...)
来源：http://dmi.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://anb.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://gtf.wangshuangyany.cn

[D09] 排序（升序）
来源：http://xfh.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://ucn.52xcode.cn

PHP:  sort($arr);
来源：http://fwq.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pic.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://the.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dzb.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://azr.hnxiangtu.top

Ruby: arr.sort
来源：http://wrv.aizwys.cn

C#:   list.Sort();
来源：http://vhm.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wcm.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eug.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pfl.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwn.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://umt.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wlp.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://san.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zvg.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hzr.pengpengdd.cyou

[D11] 反转数组
来源：http://aiv.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://cks.c1oappe.top

PHP:  array_reverse($arr);
来源：http://ndg.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hhh.52xcode.cn

TS:   [...arr].reverse();
来源：http://xfb.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://rqb.hammf.cn

Go:   slices.Reverse(arr)
来源：http://yii.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://lck.ydzc1.top

C#:   list.Reverse();
来源：http://mac.bbcook.cn

[D12] 查找元素下标
来源：http://eep.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://ptu.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://itg.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tot.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzy.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wgx.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://bet.fehbvm.com

Ruby: arr.index(x)
来源：http://fgk.c1oappe.top

C#:   list.IndexOf(x);
来源：http://yio.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://fdt.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://afz.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lca.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://lem.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://uwd.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jgd.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ayn.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hsh.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nxv.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://xub.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cqw.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qlf.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://jcs.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://suq.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rvn.nanxuanxn.top

Go:   // 手写循环
来源：http://ahf.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://bru.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ppr.uphjek.com

[D15] 去重
来源：http://ghw.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dol.yj20258888.top

PHP:  array_unique($arr);
来源：http://dha.yueranfly.top

JS:   [...new Set(arr)]
来源：http://hqx.xuanzx.com

TS:   [...new Set(arr)]
来源：http://jwg.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wmx.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://far.shuidangran.top

Ruby: arr.uniq
来源：http://aob.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://mnf.jianghu66.top

[D16] 求和与平均值
来源：http://gde.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rmm.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yhr.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ueq.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpl.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqh.tian-w.cn

Go:   // 手写循环累加
来源：http://wyj.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jlg.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://nxj.jianghu66.top

[D17] 最大值与最小值
来源：http://rbr.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://krf.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://zuk.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dqq.meibo888.top

TS:   Math.max(...arr);
来源：http://vez.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cqu.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gnq.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://uyr.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://oga.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://wtn.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://slg.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://hhf.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nht.pengpengdd.cyou

TS:   nested.flat();
来源：http://zqz.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mtq.nanxuanxn.top

Go:   // 手写双层循环
来源：http://ghd.meibo888.top

Ruby: nested.flatten
来源：http://hji.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xkl.hysaishi.cn

[D19] 按字段分组
来源：http://yau.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zve.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ijm.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aha.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://iev.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mxt.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://vke.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bgu.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wdq.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://zfa.zhijiandao.cn

Py:   Counter(arr)
来源：http://wmp.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://zdf.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oli.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iht.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://elh.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://bpl.hywenlv.cn

Ruby: arr.tally
来源：http://nah.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swl.fehbvm.com

[D21] 判断是否包含某元素
来源：http://lqz.c1oappe.top

Py:   x in arr
来源：http://lvk.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://vbf.hesvh.cn

JS:   arr.includes(x)
来源：http://rur.zhengqikj.top

TS:   arr.includes(x)
来源：http://yny.bjfxy.top

Java: list.contains(x)
来源：http://hsj.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://tio.sweek.top

Ruby: arr.include?(x)
来源：http://zic.yonumen.top

C#:   list.Contains(x)
来源：http://wif.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://vee.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zig.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://stb.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xxw.yj20258888.top

TS:   [...arr];
来源：http://kjb.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://ypi.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://idn.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://khr.yongpay.top

C#:   new List<int>(list);
来源：http://ssl.c1oappe.top

[D23] reduce 累积计算
来源：http://huy.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fvh.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kpi.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bva.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://djf.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://gxy.svipenyu.cn

Go:   // 手写循环
来源：http://oax.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ord.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://knu.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://jmp.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://say.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nhk.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ntd.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vce.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tyw.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ypp.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcl.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mcb.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://ydb.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tse.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iqe.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jtc.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yom.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qua.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jta.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qtf.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cal.cucudq.cn

[D26] 数组转字符串
来源：http://nzx.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://reo.meibo888.top

PHP:  implode(", ", $arr);
来源：http://glo.guannengcc.top

JS:   arr.join(", ")
来源：http://vai.gzhubu.top

TS:   arr.join(", ")
来源：http://ssq.nanxinkj.top

Java: String.join(", ", list)
来源：http://psw.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://jzi.yj20258.top

Ruby: arr.join(", ")
来源：http://cmc.andypj.xyz

C#:   string.Join(", ", list)
来源：http://zfb.xingfuxueyuan.xyz

================================================================================
来源：http://sko.xziqi.cn

E. 字符串处理
来源：http://znn.yueranfly.top

================================================================================
来源：http://ljj.zhoulong.xyz

[E01] 拼接字符串
来源：http://xdh.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xxq.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oqo.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzw.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pjw.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jwx.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jed.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://efu.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://myz.sysykeji.top

[E02] 重复字符串
来源：http://pve.pycfn.com

Py:   "ab" * 3
来源：http://lqf.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://nnf.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://ggz.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://omi.cheryme.top

Java: "ab".repeat(3)
来源：http://mwc.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://pmk.snrcjt.cn

Ruby: "ab" * 3
来源：http://kru.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hag.guannengcc.top

[E03] 截取子串
来源：http://gzt.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dav.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jwm.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sos.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://yhw.xinyue.icu

Java: s.substring(1, 4)
来源：http://gyz.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://shy.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dbv.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://alz.jianghu66.top

[E04] 查找子串位置
来源：http://cjc.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://xqg.sxryk.cn

PHP:  strpos($s, "x");
来源：http://elz.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gog.mhx1999.top

TS:   s.indexOf("x")
来源：http://ohs.uphjek.com

Java: s.indexOf("x")
来源：http://clw.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://iyp.xuetiantiany.cn

Ruby: s.index("x")
来源：http://tuo.wangdashe.top

C#:   s.IndexOf("x")
来源：http://rss.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cxb.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jmd.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ewk.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ycr.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yxa.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sjr.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nrg.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qfs.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mfb.xuetiantiany.cn

[E06] 替换子串
来源：http://law.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bqz.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://brp.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://quc.smart0.xyz


<!-- 参考信息 -->