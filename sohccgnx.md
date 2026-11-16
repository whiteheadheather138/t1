代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tde.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://dzn.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qlb.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://qqi.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qgl.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://txp.yj20258.top

Java: // 无解构
来源：http://gtx.hesvh.cn

Go:   // 无解构
来源：http://alu.sweek.top

Ruby: a, b = pair
来源：http://lys.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://uqz.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://dlt.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rlj.sxryk.cn

PHP:  // 无重载
来源：http://ejt.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iiv.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://awb.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sts.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://rin.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://uus.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://icv.316326.xyz

================================================================================
来源：http://mjh.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://hsv.chenjidiqi.icu

================================================================================
来源：http://iaz.nwbrower.top

[D01] 创建数组 / 列表
来源：http://nmx.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pxq.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pth.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iun.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://prq.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yhh.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://jzt.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://ucx.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lvd.cashguo.top

[D02] 追加元素到末尾
来源：http://fpy.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tek.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://znb.sysykeji.top

JS:   arr.push(4);
来源：http://txx.ppjwa.cn

TS:   arr.push(4);
来源：http://evi.jqgfzy.top

Java: list.add(4);
来源：http://gkf.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://jsh.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://izf.bbcook.cn

C#:   list.Add(4);
来源：http://tpb.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://bcl.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://sxw.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dza.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hei.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://wcm.aizwys.cn

Java: list.add(0, 0);
来源：http://eqt.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kra.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rud.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://jhx.ydzc1.top

[D04] 删除元素
来源：http://rrx.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lut.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xtr.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ywb.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://zul.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wop.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ixx.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://owa.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xxt.cqqwz.cn

[D05] 访问与修改元素
来源：http://muy.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tar.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://krh.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qvq.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://rrs.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://iib.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://hau.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rrg.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kzr.ehwqpu.com

[D06] 数组长度
来源：http://xrs.sjlbkw.cn

Py:   len(arr)
来源：http://khk.hnqzz.top

PHP:  count($arr);
来源：http://xvq.ehwqpu.com

JS:   arr.length
来源：http://qjp.jinghuilouyu.cn

TS:   arr.length
来源：http://nom.yj202588.top

Java: list.size();
来源：http://ujj.daxiang520.top

Go:   len(arr)
来源：http://ggt.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://vjd.yonumen.top

C#:   list.Count;
来源：http://iaj.mhx1999.top

[D07] 切片 / 取子数组
来源：http://ghe.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hwc.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://voe.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://ckg.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://nfa.havefunace.top

Java: list.subList(1, 4);
来源：http://pbg.mhx1999.top

Go:   arr[1:4]
来源：http://fgr.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://tna.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://dld.xziqi.cn

[D08] 合并两个数组
来源：http://ngf.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://tmh.havefunace.top

PHP:  array_merge($a, $b);
来源：http://iuu.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qsq.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://xoj.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fqg.aizwys.cn

Go:   append(a, b...)
来源：http://dnr.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://zoj.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://yel.sxryk.cn

[D09] 排序（升序）
来源：http://shg.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://qhj.jianghu66.top

PHP:  sort($arr);
来源：http://hmw.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nao.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cge.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uaf.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lnc.chenzaomai.com

Ruby: arr.sort
来源：http://inh.ppjwa.cn

C#:   list.Sort();
来源：http://fyq.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://plk.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tic.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqq.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mbb.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsc.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tfy.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://orn.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ksz.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cfv.hongshengwenyu.top

[D11] 反转数组
来源：http://aeu.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://scq.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://gbv.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dxy.ctjpmb.com

TS:   [...arr].reverse();
来源：http://brn.birdmap.top

Java: Collections.reverse(list);
来源：http://olt.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://hnl.kuanghao11.cn

Ruby: arr.reverse
来源：http://ifo.hongshengwenyu.top

C#:   list.Reverse();
来源：http://rpy.ybcxt.top

[D12] 查找元素下标
来源：http://ius.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://uni.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://juu.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyh.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mov.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbe.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://zoz.vehdjk.com

Ruby: arr.index(x)
来源：http://qqq.yuxming.cn

C#:   list.IndexOf(x);
来源：http://imy.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://tso.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dxj.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://egn.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://msf.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sml.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gkc.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://afr.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ale.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://xzt.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rcf.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sfq.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://ngt.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://rog.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://njg.sufxvd.cn

Go:   // 手写循环
来源：http://gbf.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://arh.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jkc.aibaodan.cn

[D15] 去重
来源：http://xem.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bci.tianlin.xyz

PHP:  array_unique($arr);
来源：http://wrd.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://hun.aizwys.cn

TS:   [...new Set(arr)]
来源：http://ziz.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pac.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://zdz.yuanzhike.top

Ruby: arr.uniq
来源：http://kzg.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://unj.dashuyun.cn

[D16] 求和与平均值
来源：http://fdw.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fyo.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wwx.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qyw.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lvb.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wok.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://rcv.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qmz.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://gqw.shzxlz.cn

[D17] 最大值与最小值
来源：http://mkk.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://rqc.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://fzs.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dlk.sysykeji.top

TS:   Math.max(...arr);
来源：http://twk.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ygo.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qxa.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://dsg.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://who.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://xnj.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pvs.yj202588.top

PHP:  array_merge(...$nested);
来源：http://sbx.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://swx.gotoacloud.top

TS:   nested.flat();
来源：http://kdl.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://njv.yj20258888.top

Go:   // 手写双层循环
来源：http://nvu.wangdashe.top

Ruby: nested.flatten
来源：http://tpm.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rtp.chenzaomai.com

[D19] 按字段分组
来源：http://dbd.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://htc.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zaj.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ezv.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ikv.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://azv.yongpay.top

Go:   // 手写 map[string][]T
来源：http://vbu.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vlb.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://udh.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://wxx.zhoulong.xyz

Py:   Counter(arr)
来源：http://eyz.hnqzz.top

PHP:  array_count_values($arr);
来源：http://vjq.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvh.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pct.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dby.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://uvs.yueranfly.top

Ruby: arr.tally
来源：http://qed.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://imx.yfazqb.com

[D21] 判断是否包含某元素
来源：http://seo.316326.xyz

Py:   x in arr
来源：http://wkq.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://lbs.jinqigfzy.top

JS:   arr.includes(x)
来源：http://wjk.cheryme.top

TS:   arr.includes(x)
来源：http://adm.hammf.cn

Java: list.contains(x)
来源：http://eaw.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://klz.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://dio.tian-w.cn

C#:   list.Contains(x)
来源：http://xtk.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://eni.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cyv.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zoi.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpw.ehwqpu.com

TS:   [...arr];
来源：http://awe.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://cfg.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://jgn.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://wqc.zhijiandao.cn

C#:   new List<int>(list);
来源：http://xbm.yueranfly.top

[D23] reduce 累积计算
来源：http://owq.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tkr.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tuf.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jbs.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmp.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mkc.chenjidiqi.icu

Go:   // 手写循环
来源：http://mgo.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gbd.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rbt.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://vip.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://igt.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hrq.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eol.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mmy.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yjc.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ien.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tji.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://viq.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://nou.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://isa.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tde.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aas.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cfb.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://alu.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zoi.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kpg.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xci.pengpengdd.cyou

[D26] 数组转字符串
来源：http://qec.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://oza.smart0.xyz

PHP:  implode(", ", $arr);
来源：http://wax.bbcook.cn

JS:   arr.join(", ")
来源：http://fgo.316326.xyz

TS:   arr.join(", ")
来源：http://ztd.hywenlv.cn

Java: String.join(", ", list)
来源：http://loi.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://uus.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://iql.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://des.jinqigufen.top

================================================================================
来源：http://sru.tian-w.cn

E. 字符串处理
来源：http://gyy.guowangkeji.top

================================================================================
来源：http://mac.zhijiandao.cn

[E01] 拼接字符串
来源：http://mhl.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gkr.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ein.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwi.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pnz.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tea.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qvt.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wvr.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mte.smart0.xyz

[E02] 重复字符串
来源：http://pgn.ehwqpu.com

Py:   "ab" * 3
来源：http://xnm.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://odc.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://eza.ydzc1.top

TS:   "ab".repeat(3)
来源：http://dfe.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://rlv.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://qnq.hnqzz.top

Ruby: "ab" * 3
来源：http://brk.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tje.hongshengwenyu.top

[E03] 截取子串
来源：http://ynt.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zuf.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aqf.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xqe.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://lgf.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://cof.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pzz.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://qtm.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://xzh.cdnleiting.top

[E04] 查找子串位置
来源：http://wkh.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://osi.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://vxj.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mwl.jyoumei.cn

TS:   s.indexOf("x")
来源：http://txq.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://zut.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://ybj.birdmap.top

Ruby: s.index("x")
来源：http://gfg.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://tgq.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvk.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qwq.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ghe.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://frp.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kff.xylfe.cn


<!-- 参考信息 -->