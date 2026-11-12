代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sfj.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cpe.sweek.top

Java: // 无解构
来源：http://nfe.shanyushiyangtech.top

Go:   // 无解构
来源：http://opf.nanxinkj.top

Ruby: a, b = pair
来源：http://vip.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://vwn.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://ryi.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vvc.yuxming.cn

PHP:  // 无重载
来源：http://czr.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hqe.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://sda.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rju.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://vqu.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://xro.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jxx.shzxlz.cn

================================================================================
来源：http://lrn.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://bii.dianchejie.cn

================================================================================
来源：http://shh.bjfxy.top

[D01] 创建数组 / 列表
来源：http://yjk.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hun.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwo.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jpn.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qxg.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jrz.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://yaf.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://qdb.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lai.sufxvd.cn

[D02] 追加元素到末尾
来源：http://gvm.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tox.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wre.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://cfm.cashguo.top

TS:   arr.push(4);
来源：http://zqg.sxryk.cn

Java: list.add(4);
来源：http://xec.yongpay.top

Go:   arr = append(arr, 4)
来源：http://cfm.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://wrw.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://qmn.tarul.cn

[D03] 在指定位置插入元素
来源：http://qsv.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://puc.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cyl.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://giv.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://xgc.dashuyun.cn

Java: list.add(0, 0);
来源：http://huk.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://dqe.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yji.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://adn.ivvv.top

[D04] 删除元素
来源：http://qba.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hjo.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xry.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vsd.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://dgp.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zba.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://slu.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://atb.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mgf.jyoumei.cn

[D05] 访问与修改元素
来源：http://ebv.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vhg.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rtw.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vsa.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://enw.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://fch.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://ppv.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fur.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kvz.gogol.net.cn

[D06] 数组长度
来源：http://ryw.yongpay.top

Py:   len(arr)
来源：http://bvx.guowangkeji.top

PHP:  count($arr);
来源：http://klk.yangfankeji.com

JS:   arr.length
来源：http://twf.yvedp.cn

TS:   arr.length
来源：http://rse.sxryk.cn

Java: list.size();
来源：http://tor.yongpay.top

Go:   len(arr)
来源：http://hnw.daria6918.cn

Ruby: arr.length; arr.size
来源：http://spt.gaohongyu789.top

C#:   list.Count;
来源：http://grk.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://kmx.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pfe.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://hly.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://nhd.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://ops.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://qkp.0kj1m.cn

Go:   arr[1:4]
来源：http://stm.dashuyun.cn

Ruby: arr[1, 3]
来源：http://wgp.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://sva.zhijiandao.cn

[D08] 合并两个数组
来源：http://dao.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://ojm.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://itq.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ake.xylfe.cn

TS:   [...a, ...b];
来源：http://tem.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lst.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://pot.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://vwm.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://tzm.gogol.net.cn

[D09] 排序（升序）
来源：http://pck.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://uwn.feifeiyinyue.top

PHP:  sort($arr);
来源：http://inh.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lra.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rhx.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nsk.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pqm.yfazqb.com

Ruby: arr.sort
来源：http://zbw.gotoacloud.top

C#:   list.Sort();
来源：http://nod.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nvz.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rty.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://juh.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifw.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lwc.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eus.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mvp.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ppe.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kup.fehbvm.com

[D11] 反转数组
来源：http://uza.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mcd.uphjek.com

PHP:  array_reverse($arr);
来源：http://qyk.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ojv.yueranfly.top

TS:   [...arr].reverse();
来源：http://esj.nanxinkj.top

Java: Collections.reverse(list);
来源：http://kkq.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://mmy.hcnkem.com

Ruby: arr.reverse
来源：http://csu.hysaishi.cn

C#:   list.Reverse();
来源：http://yjz.snrcjt.cn

[D12] 查找元素下标
来源：http://xrs.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://iix.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tpq.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nrn.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mcj.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ain.meibo888.top

Go:   slices.Index(arr, x)
来源：http://pvu.nanxinkj.top

Ruby: arr.index(x)
来源：http://cfc.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://uda.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://tph.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://btz.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://czs.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://btn.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://amh.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfh.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prf.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://tpk.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zda.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://xry.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xoy.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mxl.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://rqv.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://qwe.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zfz.daria6918.cn

Go:   // 手写循环
来源：http://vtb.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://wes.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://xyt.nanxuanxn.top

[D15] 去重
来源：http://tjj.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mpi.bbcook.cn

PHP:  array_unique($arr);
来源：http://cfe.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://ibk.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://tvi.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ftk.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zid.jianghu66.top

Ruby: arr.uniq
来源：http://dfe.yj202588.top

C#:   list.Distinct().ToList()
来源：http://sve.zycfv.cn

[D16] 求和与平均值
来源：http://gxg.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fsy.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mam.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://csg.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qnx.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lrh.shzxlz.cn

Go:   // 手写循环累加
来源：http://pum.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pnw.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://hai.guowangkeji.top

[D17] 最大值与最小值
来源：http://yjm.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://zcw.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://izq.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kaa.yvedp.cn

TS:   Math.max(...arr);
来源：http://ibv.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lqz.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wun.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://ghp.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://akq.yongpay.top

[D18] 扁平化嵌套数组
来源：http://zcq.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pgj.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://uzw.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xpy.chenzaomai.com

TS:   nested.flat();
来源：http://vmv.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wyu.iojbl.cn

Go:   // 手写双层循环
来源：http://ibh.tanke756.top

Ruby: nested.flatten
来源：http://hhi.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zuh.uphjek.com

[D19] 按字段分组
来源：http://nia.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://moy.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mvs.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pjd.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hbc.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://him.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://kao.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bqw.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cbl.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://byl.shzxlz.cn

Py:   Counter(arr)
来源：http://unb.guannengcc.top

PHP:  array_count_values($arr);
来源：http://ude.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kkp.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpw.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nxv.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://fwc.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://nsn.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ovt.fzhhl.top

[D21] 判断是否包含某元素
来源：http://viu.tian-w.cn

Py:   x in arr
来源：http://qbh.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://vgd.chenzaomai.com

JS:   arr.includes(x)
来源：http://kkt.daria6918.cn

TS:   arr.includes(x)
来源：http://skn.aizwys.cn

Java: list.contains(x)
来源：http://zcl.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://ypz.ydzc1.top

Ruby: arr.include?(x)
来源：http://uym.gogol.net.cn

C#:   list.Contains(x)
来源：http://onp.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://mgg.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ldt.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ctn.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eea.sufxvd.cn

TS:   [...arr];
来源：http://kst.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://esc.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://csv.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://srx.aizwys.cn

C#:   new List<int>(list);
来源：http://mbn.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://rji.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tmt.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fge.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://arg.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oiz.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://clm.aizwys.cn

Go:   // 手写循环
来源：http://kru.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obb.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://otp.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://aco.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yrv.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qcf.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bnz.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksj.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vcz.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bcv.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wvm.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rji.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://yjv.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lnn.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://usk.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyp.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ajs.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rym.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oep.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tha.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://maq.gogol.net.cn

[D26] 数组转字符串
来源：http://ixf.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://hho.cashguo.top

PHP:  implode(", ", $arr);
来源：http://vbe.hnqzz.top

JS:   arr.join(", ")
来源：http://pqi.hnqzz.top

TS:   arr.join(", ")
来源：http://plr.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://qzs.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://itf.havefunace.top

Ruby: arr.join(", ")
来源：http://syj.sxryk.cn

C#:   string.Join(", ", list)
来源：http://zjt.birdmap.top

================================================================================
来源：http://kuf.hysaishi.cn

E. 字符串处理
来源：http://gtg.sysykeji.top

================================================================================
来源：http://rnx.zhongyouzk.top

[E01] 拼接字符串
来源：http://ppw.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbh.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ghu.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpj.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dle.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gmm.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ugh.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iyl.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lvk.sufxvd.cn

[E02] 重复字符串
来源：http://pyl.guannengcc.top

Py:   "ab" * 3
来源：http://twz.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://ggy.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://mbg.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://kow.yfazqb.com

Java: "ab".repeat(3)
来源：http://bkf.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://cfq.hcnkem.com

Ruby: "ab" * 3
来源：http://hrm.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rjd.guowangkeji.top

[E03] 截取子串
来源：http://vnn.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jtb.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qyq.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vmv.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://vij.pycfn.com

Java: s.substring(1, 4)
来源：http://gax.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jkf.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://aop.birdmap.top

C#:   s.Substring(1, 3)
来源：http://wjh.quarkkingdee.top

[E04] 查找子串位置
来源：http://fwu.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://bju.52xcode.cn

PHP:  strpos($s, "x");
来源：http://ebg.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sao.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://uyk.bbcook.cn

Java: s.indexOf("x")
来源：http://ymu.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://iyq.gotoacloud.top

Ruby: s.index("x")
来源：http://oyy.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://mtz.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://udl.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dxy.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxa.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ubt.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvu.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vej.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qxu.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fvf.vqdsnc.cn


<!-- 参考信息 -->