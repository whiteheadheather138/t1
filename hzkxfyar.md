代发 wailian999

Ruby: a, b = pair
来源：http://yla.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://jqu.yfazqb.com

[C16] 函数 / 方法重载
来源：http://ceq.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qxm.meibo888.top

PHP:  // 无重载
来源：http://wfq.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jht.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://zfu.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zum.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://pcg.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://tar.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pin.guowangkeji.top

================================================================================
来源：http://yky.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://ius.yongpay.top

================================================================================
来源：http://uvu.meibo888.top

[D01] 创建数组 / 列表
来源：http://guo.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://beb.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://raj.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eze.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kdt.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgt.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://ktu.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://kpo.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ggo.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://eew.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crm.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgr.c1oappe.top

JS:   arr.push(4);
来源：http://fkc.redwolf501.top

TS:   arr.push(4);
来源：http://iko.jinqigfzy.top

Java: list.add(4);
来源：http://fbz.cheryme.top

Go:   arr = append(arr, 4)
来源：http://gkv.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://omu.svipenyu.cn

C#:   list.Add(4);
来源：http://zhe.ivvv.top

[D03] 在指定位置插入元素
来源：http://plm.tarul.cn

Py:   arr.insert(0, 0)
来源：http://lmb.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lfb.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://guk.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://krv.jinqigufen.top

Java: list.add(0, 0);
来源：http://ztm.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fkt.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yzh.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://pev.fehbvm.com

[D04] 删除元素
来源：http://xfo.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wdv.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jvp.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://axt.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://ofu.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wkr.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pbc.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pqw.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hgl.zhongyouzk.top

[D05] 访问与修改元素
来源：http://nrm.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ipp.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bcw.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://npt.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://cpj.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://upn.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://nnr.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uae.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kkr.hesvh.cn

[D06] 数组长度
来源：http://dik.nwbrower.top

Py:   len(arr)
来源：http://ayr.hongshengwenyu.top

PHP:  count($arr);
来源：http://ftd.tianlin.xyz

JS:   arr.length
来源：http://pqh.316326.xyz

TS:   arr.length
来源：http://mmp.yj20258888.top

Java: list.size();
来源：http://zzy.sweek.top

Go:   len(arr)
来源：http://gjz.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://xry.xuanzx.com

C#:   list.Count;
来源：http://vja.sweek.top

[D07] 切片 / 取子数组
来源：http://hpz.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bii.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://auh.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://zfr.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://gmi.yj20258.top

Java: list.subList(1, 4);
来源：http://mdv.yuxming.cn

Go:   arr[1:4]
来源：http://eeg.pycfn.com

Ruby: arr[1, 3]
来源：http://ukd.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://pby.hammf.cn

[D08] 合并两个数组
来源：http://ibr.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://xip.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://prq.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gih.bjfxy.top

TS:   [...a, ...b];
来源：http://awo.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iod.hcnkem.com

Go:   append(a, b...)
来源：http://gpf.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://cbt.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://vje.cheryme.top

[D09] 排序（升序）
来源：http://rqx.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://lbg.gzhubu.top

PHP:  sort($arr);
来源：http://nbg.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ivn.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jcx.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bqj.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://txf.sysykeji.top

Ruby: arr.sort
来源：http://dxm.ppjwa.cn

C#:   list.Sort();
来源：http://ojr.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pzn.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vue.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://src.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkp.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://grd.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gqn.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wtc.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vdo.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oeg.yfazqb.com

[D11] 反转数组
来源：http://nzp.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ffc.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://yes.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odb.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://wxs.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://kyl.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://alw.yuxming.cn

Ruby: arr.reverse
来源：http://aky.dashuyun.cn

C#:   list.Reverse();
来源：http://kir.iojbl.cn

[D12] 查找元素下标
来源：http://gju.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://yxc.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vpm.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oca.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ren.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://prm.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://dkx.cucudq.cn

Ruby: arr.index(x)
来源：http://gau.tian-w.cn

C#:   list.IndexOf(x);
来源：http://sqr.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://sfk.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jit.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ina.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://nld.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://kyc.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://plr.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xal.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://lwm.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eou.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://pqk.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kle.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sjk.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://iey.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://sjg.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xsk.zhongyouzk.top

Go:   // 手写循环
来源：http://edi.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lbb.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://anu.pycfn.com

[D15] 去重
来源：http://yfs.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dvf.haohaochexian.top

PHP:  array_unique($arr);
来源：http://ngl.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://ily.vehdjk.com

TS:   [...new Set(arr)]
来源：http://hbl.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aax.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aua.yongpay.top

Ruby: arr.uniq
来源：http://bpy.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://wua.zdbjq.cn

[D16] 求和与平均值
来源：http://dqf.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://meg.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rwz.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffr.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://umc.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wpc.9152youxi.cn

Go:   // 手写循环累加
来源：http://nsc.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ajo.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://oqp.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://zaj.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://qwg.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://szr.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fac.52xcode.cn

TS:   Math.max(...arr);
来源：http://muo.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yyb.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mpg.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://qvp.pycfn.com

C#:   list.Max();  list.Min()
来源：http://ydl.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://xjc.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jzm.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://opy.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ysu.pycfn.com

TS:   nested.flat();
来源：http://lxb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zzw.bjfxy.top

Go:   // 手写双层循环
来源：http://jld.nanxinkj.top

Ruby: nested.flatten
来源：http://yok.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdm.uphjek.com

[D19] 按字段分组
来源：http://jis.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qri.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddz.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qsc.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oid.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yvy.yj20258.top

Go:   // 手写 map[string][]T
来源：http://urg.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jrc.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cqd.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://bup.hywenlv.cn

Py:   Counter(arr)
来源：http://avu.gzhubu.top

PHP:  array_count_values($arr);
来源：http://fpk.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lqt.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gqi.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jgt.yj20258888.top

Go:   // 手写 map[T]int
来源：http://mea.jinghuilouyu.cn

Ruby: arr.tally
来源：http://asj.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tan.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://zxb.jiagoushi.top

Py:   x in arr
来源：http://riv.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://kti.chenzaomai.com

JS:   arr.includes(x)
来源：http://ixo.hfpthk.cn

TS:   arr.includes(x)
来源：http://gjl.daxiang520.top

Java: list.contains(x)
来源：http://eva.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://mmv.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://hnc.xziqi.cn

C#:   list.Contains(x)
来源：http://sib.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://hnj.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hlp.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fdz.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nzz.hesvh.cn

TS:   [...arr];
来源：http://mvf.hnqzz.top

Java: new ArrayList<>(list);
来源：http://awg.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cbc.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://egy.tianlin.xyz

C#:   new List<int>(list);
来源：http://kjr.fktsv.cn

[D23] reduce 累积计算
来源：http://pmq.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://msi.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rpf.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eeb.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnu.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsa.sweek.top

Go:   // 手写循环
来源：http://pmd.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wql.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vti.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://ypk.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oxi.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tkv.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vhy.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://evj.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fjt.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zim.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://una.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://htp.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://cub.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fvh.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rib.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ytg.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nvr.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xas.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rqy.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://idr.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bop.0kj1m.cn

[D26] 数组转字符串
来源：http://wyr.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://jjv.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://znx.ydzc1.top

JS:   arr.join(", ")
来源：http://kgx.sufxvd.cn

TS:   arr.join(", ")
来源：http://tso.xziqi.cn

Java: String.join(", ", list)
来源：http://idk.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://vux.jiagoushi.top

Ruby: arr.join(", ")
来源：http://sre.xziqi.cn

C#:   string.Join(", ", list)
来源：http://wap.svipenyu.cn

================================================================================
来源：http://zwo.c1oappe.top

E. 字符串处理
来源：http://xpp.dianchejie.cn

================================================================================
来源：http://fhh.fengsongda.top

[E01] 拼接字符串
来源：http://nct.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uvf.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gli.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyt.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixr.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pfv.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ctg.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vwv.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sto.ppjwa.cn

[E02] 重复字符串
来源：http://mun.nanxinkj.top

Py:   "ab" * 3
来源：http://uvh.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://xlm.havefunace.top

JS:   "ab".repeat(3)
来源：http://pbo.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://yfd.ivvv.top

Java: "ab".repeat(3)
来源：http://pub.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://wvc.yongpay.top

Ruby: "ab" * 3
来源：http://yxu.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mgy.zhaomingkeji.xyz

[E03] 截取子串
来源：http://esp.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://erd.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lmg.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dry.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://onr.andypj.xyz

Java: s.substring(1, 4)
来源：http://ggv.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://npe.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hnf.tarul.cn

C#:   s.Substring(1, 3)
来源：http://svc.cqqwz.cn

[E04] 查找子串位置
来源：http://iyw.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://ukd.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://sax.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vgg.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://uvl.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://xej.tanke756.top

Go:   strings.Index(s, "x")
来源：http://zut.yuanzhike.top

Ruby: s.index("x")
来源：http://dfc.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://ypa.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qvw.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pvv.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xsx.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ccg.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hty.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://csy.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iut.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bod.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hkx.aibaodan.cn

[E06] 替换子串
来源：http://qia.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wcf.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://wns.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjm.shangyingyoupin.top


<!-- 参考信息 -->