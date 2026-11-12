代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vca.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://qdz.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qsl.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://hki.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wwy.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://htd.xuanzx.com

Java: // 无解构
来源：http://nrt.fehbvm.com

Go:   // 无解构
来源：http://pla.gogol.net.cn

Ruby: a, b = pair
来源：http://qjn.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://vch.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://mko.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nqs.ybcxt.top

PHP:  // 无重载
来源：http://ene.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uaq.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://mbo.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nhs.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://pkh.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://vtu.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ntc.fehbvm.com

================================================================================
来源：http://hdl.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://ovu.guowangkeji.top

================================================================================
来源：http://ran.cheryme.top

[D01] 创建数组 / 列表
来源：http://bcn.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://guz.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ayw.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nsl.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zbk.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rbd.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://pam.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://zlr.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwe.ivvv.top

[D02] 追加元素到末尾
来源：http://upf.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://paz.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knd.fktsv.cn

JS:   arr.push(4);
来源：http://vlg.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://shm.52xcode.cn

Java: list.add(4);
来源：http://zkl.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://baa.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://jlh.yuxming.cn

C#:   list.Add(4);
来源：http://qdc.uphjek.com

[D03] 在指定位置插入元素
来源：http://hrl.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://fkq.nwbrower.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xve.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bcx.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://slx.yj20258888.top

Java: list.add(0, 0);
来源：http://zgo.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://fih.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gmy.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://ezn.jianghu66.top

[D04] 删除元素
来源：http://mdm.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vfb.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zrq.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aba.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://anz.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://opy.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bjy.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://svt.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://izs.sjlbkw.cn

[D05] 访问与修改元素
来源：http://frw.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://noz.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jve.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ypy.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://bcb.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://qnq.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://dhm.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pyb.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pvv.zhengqikj.top

[D06] 数组长度
来源：http://cag.hnqzz.top

Py:   len(arr)
来源：http://phd.hnxiangtu.top

PHP:  count($arr);
来源：http://egb.mhx1999.top

JS:   arr.length
来源：http://pam.epnwcf.com

TS:   arr.length
来源：http://qhm.cashguo.top

Java: list.size();
来源：http://tcq.cheryme.top

Go:   len(arr)
来源：http://cvu.52xcode.cn

Ruby: arr.length; arr.size
来源：http://cdf.xinyue.icu

C#:   list.Count;
来源：http://xip.havefunace.top

[D07] 切片 / 取子数组
来源：http://oea.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pjp.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://yng.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://lgm.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://mav.aibaodan.cn

Java: list.subList(1, 4);
来源：http://ciu.sweek.top

Go:   arr[1:4]
来源：http://wbv.fehbvm.com

Ruby: arr[1, 3]
来源：http://eal.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://svn.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://uyv.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://oxq.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://egq.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dua.cashguo.top

TS:   [...a, ...b];
来源：http://lbx.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aeg.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://mfq.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://juy.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://qdv.zycfv.cn

[D09] 排序（升序）
来源：http://anf.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://jhm.vqdsnc.cn

PHP:  sort($arr);
来源：http://sao.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bma.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tiq.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cbg.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://icq.jianghu66.top

Ruby: arr.sort
来源：http://ajg.tian-w.cn

C#:   list.Sort();
来源：http://aof.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gbv.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fvt.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xzj.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpe.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eca.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pav.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://anl.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqu.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xeh.jqgfzy.top

[D11] 反转数组
来源：http://kxh.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tkm.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://vny.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ggq.yfazqb.com

TS:   [...arr].reverse();
来源：http://mbz.fehbvm.com

Java: Collections.reverse(list);
来源：http://oqm.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://tqr.zdqjudy.top

Ruby: arr.reverse
来源：http://jcx.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://uzm.andypj.xyz

[D12] 查找元素下标
来源：http://hko.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://opo.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ocn.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bie.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mwz.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zvo.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://ghh.ivvv.top

Ruby: arr.index(x)
来源：http://lti.cashguo.top

C#:   list.IndexOf(x);
来源：http://nzd.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://pfs.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zdi.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://esf.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://grm.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://lsv.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gsx.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iso.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://dsh.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gef.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://jgr.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hvz.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fvf.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://zjg.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://rnh.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ozw.hnxiangtu.top

Go:   // 手写循环
来源：http://rph.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tda.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dnh.zhaomingkeji.xyz

[D15] 去重
来源：http://fei.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sfs.epnwcf.com

PHP:  array_unique($arr);
来源：http://ypw.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://ibn.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://eck.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hcu.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://iha.9152youxi.cn

Ruby: arr.uniq
来源：http://zpw.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://ibq.quarkkingdee.top

[D16] 求和与平均值
来源：http://hpu.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hbm.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pwe.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://chx.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfl.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sjb.jlsjyb.cn

Go:   // 手写循环累加
来源：http://ioy.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://evg.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://vbi.chenzaomai.com

[D17] 最大值与最小值
来源：http://bnc.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://sbx.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://ahe.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ben.sxryk.cn

TS:   Math.max(...arr);
来源：http://saf.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ixz.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsg.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://flw.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://hoo.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://duw.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ksz.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://vka.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dha.jqgfzy.top

TS:   nested.flat();
来源：http://zdo.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hrw.cqqwz.cn

Go:   // 手写双层循环
来源：http://vsn.gogol.net.cn

Ruby: nested.flatten
来源：http://yuk.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://fsf.tanke756.top

[D19] 按字段分组
来源：http://jik.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://slk.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqy.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xxy.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rzi.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dpx.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://mbc.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tqh.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://arj.birdmap.top

[D20] 统计每个元素出现次数
来源：http://zko.hammf.cn

Py:   Counter(arr)
来源：http://nky.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://vxm.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mtg.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rmg.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sjk.daria6918.cn

Go:   // 手写 map[T]int
来源：http://cps.chenlongwang.top

Ruby: arr.tally
来源：http://bym.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ecc.iojbl.cn

[D21] 判断是否包含某元素
来源：http://jbg.iojbl.cn

Py:   x in arr
来源：http://ybk.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://nxn.yueranfly.top

JS:   arr.includes(x)
来源：http://yzf.hammf.cn

TS:   arr.includes(x)
来源：http://ink.zdqjudy.top

Java: list.contains(x)
来源：http://cuz.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://ldv.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://wvx.xuanzx.com

C#:   list.Contains(x)
来源：http://tye.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://iwp.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zrx.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gyu.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://upe.zhongyouzk.top

TS:   [...arr];
来源：http://ozl.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://zor.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nij.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://vdj.yongpay.top

C#:   new List<int>(list);
来源：http://qwv.cdnleiting.top

[D23] reduce 累积计算
来源：http://rlm.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://boe.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xgl.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovq.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xrh.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zxv.yfazqb.com

Go:   // 手写循环
来源：http://miq.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hkp.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tdo.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://vfu.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tfx.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rrc.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbn.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://juy.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xnp.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nrs.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nqn.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xhq.yj20258.top

[D25] Set 集合去重与交并差
来源：http://gdw.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wug.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://esg.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zmh.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cox.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cwt.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ggm.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vih.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ivk.0kj1m.cn

[D26] 数组转字符串
来源：http://lta.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://vnd.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://kar.guowangkeji.top

JS:   arr.join(", ")
来源：http://fmy.zhongyouzk.top

TS:   arr.join(", ")
来源：http://dte.zhongyouzk.top

Java: String.join(", ", list)
来源：http://tnq.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://wcg.cqqwz.cn

Ruby: arr.join(", ")
来源：http://ipu.cheryme.top

C#:   string.Join(", ", list)
来源：http://lvg.316326.xyz

================================================================================
来源：http://dvq.uphjek.com

E. 字符串处理
来源：http://ryp.snrcjt.cn

================================================================================
来源：http://luh.yuanzhike.top

[E01] 拼接字符串
来源：http://rol.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pmt.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pvj.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zol.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyb.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wsl.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://spq.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwp.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gsq.zhoulong.xyz

[E02] 重复字符串
来源：http://syv.bjfxy.top

Py:   "ab" * 3
来源：http://gsi.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://bey.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://suj.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://bce.redwolf501.top

Java: "ab".repeat(3)
来源：http://izq.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://nfv.havefunace.top

Ruby: "ab" * 3
来源：http://ulz.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yft.gogol.net.cn

[E03] 截取子串
来源：http://oqh.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wqz.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zff.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jxv.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://qvc.redwolf501.top

Java: s.substring(1, 4)
来源：http://stl.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xoq.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hjh.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://pue.tanke756.top

[E04] 查找子串位置
来源：http://osa.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://kgr.yfazqb.com

PHP:  strpos($s, "x");
来源：http://ejq.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://drd.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://zwo.cashguo.top

Java: s.indexOf("x")
来源：http://nxp.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://dfc.zhiwuduotai.top

Ruby: s.index("x")
来源：http://lbb.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://lni.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://wmc.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jzc.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hjo.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wba.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nio.cashguo.top


<!-- 参考信息 -->