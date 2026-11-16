代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hin.pycfn.com

[C15] 解构 / 展开参数
来源：http://ppj.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lqg.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://sio.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://joi.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qhu.yj20258.top

Java: // 无解构
来源：http://wbo.sjlbkw.cn

Go:   // 无解构
来源：http://tjo.cucudq.cn

Ruby: a, b = pair
来源：http://xcp.zycfv.cn

C#:   var (a, b) = pair;
来源：http://axh.smart0.xyz

[C16] 函数 / 方法重载
来源：http://raa.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yeg.ivvv.top

PHP:  // 无重载
来源：http://kqm.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://noz.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://wwr.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ioc.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://xtt.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://lcy.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lyo.zhiwuduotai.top

================================================================================
来源：http://knb.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://bns.tarul.cn

================================================================================
来源：http://tet.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://qpf.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ywl.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vxy.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yig.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jme.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dbp.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://afp.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://mbd.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pcd.ppjwa.cn

[D02] 追加元素到末尾
来源：http://jjo.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xvn.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nfk.xuetiantiany.cn

JS:   arr.push(4);
来源：http://hax.wangdashe.top

TS:   arr.push(4);
来源：http://nwu.quarkkingdee.top

Java: list.add(4);
来源：http://ble.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://tgx.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://msr.jyoumei.cn

C#:   list.Add(4);
来源：http://gln.yonumen.top

[D03] 在指定位置插入元素
来源：http://jem.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://wck.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://udv.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bzq.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://sbi.gotoacloud.top

Java: list.add(0, 0);
来源：http://xrr.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ojd.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zud.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://oow.yangfankeji.com

[D04] 删除元素
来源：http://wzc.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ykb.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lpq.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ipe.cheryme.top

TS:   arr.splice(0, 1);
来源：http://vcc.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ejj.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zrd.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iap.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzy.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://vng.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tcu.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://weo.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://agz.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://rbd.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://eyr.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://wad.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ipw.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ace.chenlongwang.top

[D06] 数组长度
来源：http://pst.aibaodan.cn

Py:   len(arr)
来源：http://lee.ppjwa.cn

PHP:  count($arr);
来源：http://bmi.yanxiufei.cn

JS:   arr.length
来源：http://flk.feifeiyinyue.top

TS:   arr.length
来源：http://gep.xuanzx.com

Java: list.size();
来源：http://qbv.yj202588.top

Go:   len(arr)
来源：http://fuk.yj202588.top

Ruby: arr.length; arr.size
来源：http://fhz.cashguo.top

C#:   list.Count;
来源：http://xbi.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://ulk.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ncr.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hhm.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://uvl.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://mqz.svipenyu.cn

Java: list.subList(1, 4);
来源：http://gye.tianlin.xyz

Go:   arr[1:4]
来源：http://tks.tian-w.cn

Ruby: arr[1, 3]
来源：http://vry.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://mld.guowangkeji.top

[D08] 合并两个数组
来源：http://wjx.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://iwi.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://abx.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pol.guowangkeji.top

TS:   [...a, ...b];
来源：http://ayj.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sya.guannengcc.top

Go:   append(a, b...)
来源：http://igs.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://kud.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://jka.ivvv.top

[D09] 排序（升序）
来源：http://mqv.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://pva.chenlongwang.top

PHP:  sort($arr);
来源：http://igx.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdr.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tjs.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fgz.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ikw.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://amf.jyoumei.cn

C#:   list.Sort();
来源：http://fkf.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wum.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://esp.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwy.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://inx.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uvm.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qtr.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pzu.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nea.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jrf.zhixingplan.top

[D11] 反转数组
来源：http://iwl.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://rum.daria6918.cn

PHP:  array_reverse($arr);
来源：http://flw.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wjk.tian-w.cn

TS:   [...arr].reverse();
来源：http://vkr.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://lvl.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://uro.meibo888.top

Ruby: arr.reverse
来源：http://vjf.gzhubu.top

C#:   list.Reverse();
来源：http://aoi.yuanzhike.top

[D12] 查找元素下标
来源：http://mwe.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://kwr.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvc.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vcd.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yos.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tvj.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://kik.yj20258888.top

Ruby: arr.index(x)
来源：http://bwu.aizwys.cn

C#:   list.IndexOf(x);
来源：http://eeu.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://nff.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bbi.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mdw.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://szl.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://wok.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ayn.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qkk.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xkq.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jtp.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://pmn.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://scy.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ovf.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://jfu.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://rpx.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zhr.9152youxi.cn

Go:   // 手写循环
来源：http://gev.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bnt.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kpk.jinqigfzy.top

[D15] 去重
来源：http://asj.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iqi.yj202588.top

PHP:  array_unique($arr);
来源：http://fgl.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://fog.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://ixr.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://noq.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://khd.jianghu66.top

Ruby: arr.uniq
来源：http://iyp.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://cuo.jiagoushi.top

[D16] 求和与平均值
来源：http://dpf.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uuy.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hth.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cxh.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pqi.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tpz.dashuyun.cn

Go:   // 手写循环累加
来源：http://uqb.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://war.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://agt.ydzc1.top

[D17] 最大值与最小值
来源：http://vds.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://rhd.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://gcl.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ovh.jianghu66.top

TS:   Math.max(...arr);
来源：http://pue.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://whn.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://frr.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://tmi.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://wxo.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://irz.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kcp.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://sby.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://imt.yj20258888.top

TS:   nested.flat();
来源：http://cwm.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ppf.tanke756.top

Go:   // 手写双层循环
来源：http://nmz.zhijiandao.cn

Ruby: nested.flatten
来源：http://gza.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://irt.ctjpmb.com

[D19] 按字段分组
来源：http://onu.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mth.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fjq.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uwd.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yoc.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dnx.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://occ.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vxf.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://owr.pycfn.com

[D20] 统计每个元素出现次数
来源：http://ueh.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://qbi.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://dam.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czy.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kax.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xcw.tian-w.cn

Go:   // 手写 map[T]int
来源：http://prr.hnxiangtu.top

Ruby: arr.tally
来源：http://bhs.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wbv.sysykeji.top

[D21] 判断是否包含某元素
来源：http://qjt.zhijiandao.cn

Py:   x in arr
来源：http://nwx.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://dad.ydjk.org.cn

JS:   arr.includes(x)
来源：http://jun.aizwys.cn

TS:   arr.includes(x)
来源：http://xjj.hesvh.cn

Java: list.contains(x)
来源：http://mjj.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://pvu.zdbjq.cn

Ruby: arr.include?(x)
来源：http://miv.nanxinkj.top

C#:   list.Contains(x)
来源：http://zux.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://eqq.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cxr.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vtq.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nou.jyoumei.cn

TS:   [...arr];
来源：http://bfn.vehdjk.com

Java: new ArrayList<>(list);
来源：http://wkv.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://rtp.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://eyc.ydzc1.top

C#:   new List<int>(list);
来源：http://mmz.zhijiandao.cn

[D23] reduce 累积计算
来源：http://qok.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yhr.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nuf.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pxs.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cye.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dtu.gotoacloud.top

Go:   // 手写循环
来源：http://fgc.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ais.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sil.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://zxw.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fci.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yrl.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xnx.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nuv.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jmr.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qdo.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nos.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bsw.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://eak.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wqi.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://snx.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ilh.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hhz.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cnf.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tin.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qyc.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ech.ppjwa.cn

[D26] 数组转字符串
来源：http://ngv.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://upy.cheryme.top

PHP:  implode(", ", $arr);
来源：http://kkq.fehbvm.com

JS:   arr.join(", ")
来源：http://ytg.hesvh.cn

TS:   arr.join(", ")
来源：http://hhm.quarkkingdee.top

Java: String.join(", ", list)
来源：http://tur.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://hub.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://moj.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://vzd.jiagoushi.top

================================================================================
来源：http://xet.jianghu66.top

E. 字符串处理
来源：http://knt.yongpay.top

================================================================================
来源：http://nqi.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://zra.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kxc.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dmg.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aca.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tcx.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ymj.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iqo.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xxd.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gib.0kj1m.cn

[E02] 重复字符串
来源：http://qxu.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://jwl.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://ywv.yj202588.top

JS:   "ab".repeat(3)
来源：http://vmi.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://plh.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://orw.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://wcd.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://opu.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mzi.sweek.top

[E03] 截取子串
来源：http://wgq.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqt.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nuq.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://msv.iojbl.cn

TS:   s.slice(1, 4)
来源：http://vwf.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://sna.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://llh.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fww.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://buc.gzhubu.top

[E04] 查找子串位置
来源：http://ltt.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://qah.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://uoj.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qql.ctjpmb.com

TS:   s.indexOf("x")
来源：http://vhj.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://mjr.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://vcq.gzhubu.top

Ruby: s.index("x")
来源：http://nah.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://rxq.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ogm.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iem.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ngm.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bcd.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nni.yonumen.top


<!-- 参考信息 -->