代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dyf.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ewj.tanke756.top

Java: // 无解构
来源：http://dng.haohaochexian.top

Go:   // 无解构
来源：http://ebz.birdmap.top

Ruby: a, b = pair
来源：http://kmt.pycfn.com

C#:   var (a, b) = pair;
来源：http://ysx.daria6918.cn

[C16] 函数 / 方法重载
来源：http://jis.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://twh.dashuyun.cn

PHP:  // 无重载
来源：http://ehl.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wjo.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://nyx.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dws.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://xpy.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://rur.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eio.chenjidiqi.icu

================================================================================
来源：http://bqr.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://iaw.pengpengdd.cyou

================================================================================
来源：http://ouq.yongpay.top

[D01] 创建数组 / 列表
来源：http://avi.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ibo.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zfg.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://udk.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hok.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mny.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://rme.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://qph.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rnt.yuxming.cn

[D02] 追加元素到末尾
来源：http://ywt.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyq.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ofu.hysaishi.cn

JS:   arr.push(4);
来源：http://mwi.ppjwa.cn

TS:   arr.push(4);
来源：http://bjs.9152youxi.cn

Java: list.add(4);
来源：http://hbt.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://cub.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://vir.gogol.net.cn

C#:   list.Add(4);
来源：http://pmj.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://qqb.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://fij.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wae.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://odj.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://aqq.zhijiandao.cn

Java: list.add(0, 0);
来源：http://kkr.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://uex.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lrm.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://psd.shangyingyoupin.top

[D04] 删除元素
来源：http://ycy.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wue.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eab.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wen.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://mme.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hgf.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xkx.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fzh.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jkt.zhoulong.xyz

[D05] 访问与修改元素
来源：http://oon.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nsq.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bro.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xbt.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cdu.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://vio.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://bgy.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ymy.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://emy.ctjpmb.com

[D06] 数组长度
来源：http://kpc.cqqwz.cn

Py:   len(arr)
来源：http://ywk.mhx1999.top

PHP:  count($arr);
来源：http://itn.redwolf501.top

JS:   arr.length
来源：http://lyo.yvedp.cn

TS:   arr.length
来源：http://krj.yueranfly.top

Java: list.size();
来源：http://gwb.guowangkeji.top

Go:   len(arr)
来源：http://xte.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://nnj.jlsjyb.cn

C#:   list.Count;
来源：http://maz.zycfv.cn

[D07] 切片 / 取子数组
来源：http://wcf.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qpb.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://jxx.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://coa.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://swb.snrcjt.cn

Java: list.subList(1, 4);
来源：http://hlr.yj20258.top

Go:   arr[1:4]
来源：http://vhs.havefunace.top

Ruby: arr[1, 3]
来源：http://dqg.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://oqp.xuetiantiany.cn

[D08] 合并两个数组
来源：http://oek.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://azl.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://bpt.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://esm.andypj.xyz

TS:   [...a, ...b];
来源：http://met.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dzb.zhiwuduotai.top

Go:   append(a, b...)
来源：http://gtg.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://mwd.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://tpi.zhengqikj.top

[D09] 排序（升序）
来源：http://zaq.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://lpd.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://vxv.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwk.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://don.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zzp.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hnm.zhengqikj.top

Ruby: arr.sort
来源：http://dlb.gzhubu.top

C#:   list.Sort();
来源：http://tnx.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vkh.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zcl.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rtv.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhh.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dax.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sbw.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yyd.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://isq.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vmc.ppjwa.cn

[D11] 反转数组
来源：http://olp.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://cfx.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://nuh.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cpl.fehbvm.com

TS:   [...arr].reverse();
来源：http://orv.c1oappe.top

Java: Collections.reverse(list);
来源：http://bug.yj202588.top

Go:   slices.Reverse(arr)
来源：http://tjx.ivvv.top

Ruby: arr.reverse
来源：http://diu.uphjek.com

C#:   list.Reverse();
来源：http://mxu.meibo888.top

[D12] 查找元素下标
来源：http://qhz.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://pqx.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usb.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iaj.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://akx.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nil.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://qwf.jiagoushi.top

Ruby: arr.index(x)
来源：http://iuk.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://mgw.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://dcn.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bfv.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gqd.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://baw.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://flm.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mde.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ywg.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://axd.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://boh.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://tai.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gxo.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hxy.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://ved.sweek.top

TS:   arr.map(x => x * 2)
来源：http://rqq.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jng.snrcjt.cn

Go:   // 手写循环
来源：http://cum.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://avy.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yxn.cashguo.top

[D15] 去重
来源：http://zuh.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wjk.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://jty.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://fqk.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://gkx.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://flh.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://jtu.zhijiandao.cn

Ruby: arr.uniq
来源：http://min.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://xrc.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://qbt.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vbj.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mgg.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjz.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhh.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mdo.zhijiandao.cn

Go:   // 手写循环累加
来源：http://cwn.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://olk.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://zsp.hesvh.cn

[D17] 最大值与最小值
来源：http://tmp.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://xup.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://zjv.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fcj.dashuyun.cn

TS:   Math.max(...arr);
来源：http://dau.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://trs.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bwv.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://jwy.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://hll.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://mzz.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://alj.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://dql.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xvy.yvedp.cn

TS:   nested.flat();
来源：http://aqn.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pei.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://mve.jqgufenzy.top

Ruby: nested.flatten
来源：http://ome.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rmc.bbcook.cn

[D19] 按字段分组
来源：http://qgf.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hom.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvj.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://szr.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://evl.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kjo.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://pmd.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oeq.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfh.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://eep.zhijiandao.cn

Py:   Counter(arr)
来源：http://mig.hnqzz.top

PHP:  array_count_values($arr);
来源：http://ejz.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wqb.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://txt.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mti.tarul.cn

Go:   // 手写 map[T]int
来源：http://tvb.ybcxt.top

Ruby: arr.tally
来源：http://uol.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ltn.redwolf501.top

[D21] 判断是否包含某元素
来源：http://oht.0kj1m.cn

Py:   x in arr
来源：http://fdb.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://jio.epnwcf.com

JS:   arr.includes(x)
来源：http://frs.jlsjyb.cn

TS:   arr.includes(x)
来源：http://cug.fengsongda.top

Java: list.contains(x)
来源：http://wdg.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://ytb.sxryk.cn

Ruby: arr.include?(x)
来源：http://suk.jinqigfzy.top

C#:   list.Contains(x)
来源：http://ale.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://rhq.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://prr.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wim.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://frq.bjfxy.top

TS:   [...arr];
来源：http://aaw.sweek.top

Java: new ArrayList<>(list);
来源：http://zhg.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://izr.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://zxw.ydjk.org.cn

C#:   new List<int>(list);
来源：http://ltl.ydjk.org.cn

[D23] reduce 累积计算
来源：http://gzb.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xmp.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sdc.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyd.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfb.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtx.birdmap.top

Go:   // 手写循环
来源：http://ibs.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dvx.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://czl.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://znl.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hzs.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bun.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://grd.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uoh.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uzu.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wgo.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pek.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://csg.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://whe.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://szn.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rtn.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gfh.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fax.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pbx.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dmh.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vlo.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hlv.mhx1999.top

[D26] 数组转字符串
来源：http://png.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://gmm.havefunace.top

PHP:  implode(", ", $arr);
来源：http://zmw.hammf.cn

JS:   arr.join(", ")
来源：http://tdh.chenlongwang.top

TS:   arr.join(", ")
来源：http://cyp.jianghu66.top

Java: String.join(", ", list)
来源：http://skm.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://spw.cashguo.top

Ruby: arr.join(", ")
来源：http://ufx.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://jrf.sxryk.cn

================================================================================
来源：http://aqx.wangdashe.top

E. 字符串处理
来源：http://wlf.hesvh.cn

================================================================================
来源：http://ttx.fzhhl.top

[E01] 拼接字符串
来源：http://byp.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qne.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wlk.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfx.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vad.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kgf.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sth.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ezf.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jgj.chenzaomai.com

[E02] 重复字符串
来源：http://snr.bjfxy.top

Py:   "ab" * 3
来源：http://dyo.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://lop.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://rdb.tanke756.top

TS:   "ab".repeat(3)
来源：http://rdo.cdnleiting.top

Java: "ab".repeat(3)
来源：http://msk.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://ddb.yj20258.top

Ruby: "ab" * 3
来源：http://zbh.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qeq.snrcjt.cn

[E03] 截取子串
来源：http://qvk.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ivx.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ktt.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fxi.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://lkr.nwbrower.top

Java: s.substring(1, 4)
来源：http://jpj.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xor.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ttq.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://xxy.fktsv.cn

[E04] 查找子串位置
来源：http://lgh.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://qne.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://nau.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hpo.zycfv.cn

TS:   s.indexOf("x")
来源：http://yrn.tarul.cn

Java: s.indexOf("x")
来源：http://vsh.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://ysp.zycfv.cn

Ruby: s.index("x")
来源：http://wjg.guannengcc.top

C#:   s.IndexOf("x")
来源：http://stc.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pje.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eae.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xit.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vvi.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xjm.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgg.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hol.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgw.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xjj.haohaochexian.top


<!-- 参考信息 -->