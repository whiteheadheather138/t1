代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tac.havefunace.top

[C15] 解构 / 展开参数
来源：http://rhw.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vfm.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://qlu.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jyq.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zch.c1oappe.top

Java: // 无解构
来源：http://iou.yuanzhike.top

Go:   // 无解构
来源：http://inu.jqgfzy.top

Ruby: a, b = pair
来源：http://aiy.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://bix.cucudq.cn

[C16] 函数 / 方法重载
来源：http://ehx.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zqi.cashguo.top

PHP:  // 无重载
来源：http://uhu.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://djv.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://dvt.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://par.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://qpo.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://cto.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzo.c1oappe.top

================================================================================
来源：http://usx.uphjek.com

D. 数组 / 列表 / 集合
来源：http://vol.uphjek.com

================================================================================
来源：http://hes.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://gas.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jak.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebz.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fan.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://brj.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xof.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://poi.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://wdn.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kai.yuxming.cn

[D02] 追加元素到末尾
来源：http://kbn.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://off.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mma.daxiang520.top

JS:   arr.push(4);
来源：http://lqh.sweek.top

TS:   arr.push(4);
来源：http://adu.andypj.xyz

Java: list.add(4);
来源：http://uja.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://bdb.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://iin.jinqigufen.top

C#:   list.Add(4);
来源：http://zcp.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://dia.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://snh.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zit.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qfp.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://vmc.fzhhl.top

Java: list.add(0, 0);
来源：http://wfd.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://biq.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sbi.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://kwz.shangyingyoupin.top

[D04] 删除元素
来源：http://wsj.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rmj.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwn.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yfv.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://wqa.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ocx.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ypj.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://stu.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ubb.0kj1m.cn

[D05] 访问与修改元素
来源：http://fef.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fas.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cim.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://huf.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://hbv.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://hyg.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://kul.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cni.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://phy.yuxming.cn

[D06] 数组长度
来源：http://fmm.ydzc1.top

Py:   len(arr)
来源：http://bcy.svipenyu.cn

PHP:  count($arr);
来源：http://pmm.daria6918.cn

JS:   arr.length
来源：http://ivh.zhongyouzk.top

TS:   arr.length
来源：http://ken.ybcxt.top

Java: list.size();
来源：http://swe.xziqi.cn

Go:   len(arr)
来源：http://lmn.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://jwc.guowangkeji.top

C#:   list.Count;
来源：http://oiu.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://kmg.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://osl.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://jjj.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://rdq.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://ppb.sysykeji.top

Java: list.subList(1, 4);
来源：http://bgi.daxiang520.top

Go:   arr[1:4]
来源：http://akd.aibaodan.cn

Ruby: arr[1, 3]
来源：http://fgb.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://vxk.jinqigufen.top

[D08] 合并两个数组
来源：http://trv.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://oyt.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://tox.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qvl.sxryk.cn

TS:   [...a, ...b];
来源：http://wzo.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://odg.meibo888.top

Go:   append(a, b...)
来源：http://udm.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://ohy.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://nwh.52xcode.cn

[D09] 排序（升序）
来源：http://rhr.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://xdd.sweek.top

PHP:  sort($arr);
来源：http://ahf.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gsn.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dco.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zjm.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qua.hfpthk.cn

Ruby: arr.sort
来源：http://pbg.shzxlz.cn

C#:   list.Sort();
来源：http://ljl.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dvs.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ycx.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eci.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gwo.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlr.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lkk.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://snf.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xvm.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zqt.jlsjyb.cn

[D11] 反转数组
来源：http://zsu.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pmb.xziqi.cn

PHP:  array_reverse($arr);
来源：http://mdx.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fjl.hesvh.cn

TS:   [...arr].reverse();
来源：http://exg.vehdjk.com

Java: Collections.reverse(list);
来源：http://icf.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://ejs.svipenyu.cn

Ruby: arr.reverse
来源：http://vdi.hfpthk.cn

C#:   list.Reverse();
来源：http://ukm.jqgufenzy.top

[D12] 查找元素下标
来源：http://rtm.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://phd.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xtq.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nah.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdv.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eds.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://ggs.dianchejie.cn

Ruby: arr.index(x)
来源：http://sow.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://xdl.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://odv.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vxf.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rju.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://xzm.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://hip.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gdl.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://izy.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://vdj.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mfr.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://ars.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vgt.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqa.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://obr.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://nes.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pko.xinyue.icu

Go:   // 手写循环
来源：http://lbz.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://wyp.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hzs.gaohongyu789.top

[D15] 去重
来源：http://dit.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mxr.yvedp.cn

PHP:  array_unique($arr);
来源：http://sdn.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://duf.xziqi.cn

TS:   [...new Set(arr)]
来源：http://kyh.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xov.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://edt.hesvh.cn

Ruby: arr.uniq
来源：http://cry.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://fen.zhixingplan.top

[D16] 求和与平均值
来源：http://kuz.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vgd.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bcv.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpy.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://map.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xyo.ybcxt.top

Go:   // 手写循环累加
来源：http://nvl.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://imo.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://ulb.fktsv.cn

[D17] 最大值与最小值
来源：http://xck.yongpay.top

Py:   max(arr);  min(arr)
来源：http://ztl.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://thh.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vkj.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://aaq.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pqb.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://etr.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://bqc.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://hxq.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://oxj.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ihs.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://wit.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://biw.jianghu66.top

TS:   nested.flat();
来源：http://kkg.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hqg.gotoacloud.top

Go:   // 手写双层循环
来源：http://dgc.cdnleiting.top

Ruby: nested.flatten
来源：http://sko.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://krh.xuanzx.com

[D19] 按字段分组
来源：http://byv.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zlr.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kjt.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xlg.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qmn.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zdr.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://ggi.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wkz.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://urp.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://mqg.vehdjk.com

Py:   Counter(arr)
来源：http://mvl.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://bey.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hwn.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ygz.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iei.yongpay.top

Go:   // 手写 map[T]int
来源：http://sgi.wangshuangyany.cn

Ruby: arr.tally
来源：http://qgi.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ola.sysykeji.top

[D21] 判断是否包含某元素
来源：http://gkt.fktsv.cn

Py:   x in arr
来源：http://qai.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://hqh.wangdashe.top

JS:   arr.includes(x)
来源：http://cul.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://gnq.pengpengdd.cyou

Java: list.contains(x)
来源：http://tth.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://rap.cdnleiting.top

Ruby: arr.include?(x)
来源：http://rlz.c1oappe.top

C#:   list.Contains(x)
来源：http://dkd.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://xjy.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rex.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rtl.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jkh.aibaodan.cn

TS:   [...arr];
来源：http://gux.ydzc1.top

Java: new ArrayList<>(list);
来源：http://vbc.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://vfb.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://sio.snrcjt.cn

C#:   new List<int>(list);
来源：http://fxi.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://qkv.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xko.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gvx.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjd.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vmh.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://twp.fzhhl.top

Go:   // 手写循环
来源：http://jrl.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obz.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xlp.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://ddz.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://amd.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jpb.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ofv.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bbz.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsm.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dyz.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cwf.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zov.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://pne.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yas.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fpg.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hti.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vzr.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwb.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ekh.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eog.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kda.chenjidiqi.icu

[D26] 数组转字符串
来源：http://zkt.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://ljh.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://tae.chenzaomai.com

JS:   arr.join(", ")
来源：http://yrq.hammf.cn

TS:   arr.join(", ")
来源：http://wph.chenlongwang.top

Java: String.join(", ", list)
来源：http://zxy.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://vty.yuanzhike.top

Ruby: arr.join(", ")
来源：http://scs.jianghu66.top

C#:   string.Join(", ", list)
来源：http://wfw.quarkkingdee.top

================================================================================
来源：http://rxf.yuanzhike.top

E. 字符串处理
来源：http://utn.jqgfzy.top

================================================================================
来源：http://yqa.cashguo.top

[E01] 拼接字符串
来源：http://lym.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bka.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://utj.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kyq.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://imd.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cbm.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://snc.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tnj.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xqd.yueranfly.top

[E02] 重复字符串
来源：http://cbc.jinqigufen.top

Py:   "ab" * 3
来源：http://uhy.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://qto.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://nwx.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://hrj.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://rqr.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://gte.havefunace.top

Ruby: "ab" * 3
来源：http://amp.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ncy.haohaochexian.top

[E03] 截取子串
来源：http://zea.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uuk.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dat.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgn.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://kgj.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://mda.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zyv.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://tqn.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://mtm.yj20258.top

[E04] 查找子串位置
来源：http://jmy.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://bpg.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://qqq.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mbj.chenzaomai.com

TS:   s.indexOf("x")
来源：http://fbe.xylfe.cn

Java: s.indexOf("x")
来源：http://yvb.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://new.yuanzhike.top

Ruby: s.index("x")
来源：http://ydy.cashguo.top

C#:   s.IndexOf("x")
来源：http://tvw.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nja.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ojj.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://njw.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aks.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://cjc.smart0.xyz


<!-- 参考信息 -->