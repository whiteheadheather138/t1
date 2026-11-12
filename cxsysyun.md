代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hwy.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zgr.zycfv.cn

Java: // 无解构
来源：http://dwx.guannengcc.top

Go:   // 无解构
来源：http://qkq.jiagoushi.top

Ruby: a, b = pair
来源：http://xvt.fengsongda.top

C#:   var (a, b) = pair;
来源：http://dxi.yueranfly.top

[C16] 函数 / 方法重载
来源：http://lje.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hys.pycfn.com

PHP:  // 无重载
来源：http://zyr.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mng.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://iqw.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dna.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://rqf.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://qrl.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://egg.tanke756.top

================================================================================
来源：http://ytg.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://nvs.dianchejie.cn

================================================================================
来源：http://fbe.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://pbb.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xda.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cyn.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brc.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mzz.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hcf.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://sjy.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://cps.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zyf.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://eol.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jtv.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xny.yonumen.top

JS:   arr.push(4);
来源：http://jaw.yanxiufei.cn

TS:   arr.push(4);
来源：http://zgj.ivvv.top

Java: list.add(4);
来源：http://ghr.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://yro.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://mdd.chenjidiqi.icu

C#:   list.Add(4);
来源：http://iod.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://ipp.pycfn.com

Py:   arr.insert(0, 0)
来源：http://lil.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://poc.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bub.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://yid.jqgfzy.top

Java: list.add(0, 0);
来源：http://kfv.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cev.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nkq.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://cfe.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://tmt.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://apo.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://quk.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fil.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://lir.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jag.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://axm.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yqe.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jmd.ybcxt.top

[D05] 访问与修改元素
来源：http://nxv.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mtw.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bee.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mit.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://lwz.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://wdx.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://igq.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zwi.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vyl.jinqigufen.top

[D06] 数组长度
来源：http://rji.bjfxy.top

Py:   len(arr)
来源：http://ztt.fzhhl.top

PHP:  count($arr);
来源：http://vib.zhaomingkeji.xyz

JS:   arr.length
来源：http://jci.snrcjt.cn

TS:   arr.length
来源：http://owr.hywenlv.cn

Java: list.size();
来源：http://gsa.zhixingplan.top

Go:   len(arr)
来源：http://wkt.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://pjp.uphjek.com

C#:   list.Count;
来源：http://pld.zycfv.cn

[D07] 切片 / 取子数组
来源：http://fin.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lpr.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jnx.meibo888.top

JS:   arr.slice(1, 4);
来源：http://lqg.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://djf.bjfxy.top

Java: list.subList(1, 4);
来源：http://bor.9152youxi.cn

Go:   arr[1:4]
来源：http://ube.hcnkem.com

Ruby: arr[1, 3]
来源：http://wfz.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://xvy.zhongyouzk.top

[D08] 合并两个数组
来源：http://bre.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://mvs.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://zaf.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mmr.dianchejie.cn

TS:   [...a, ...b];
来源：http://cgh.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hpb.zhengqikj.top

Go:   append(a, b...)
来源：http://rop.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://ibs.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://hed.cdnleiting.top

[D09] 排序（升序）
来源：http://sui.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ouv.redwolf501.top

PHP:  sort($arr);
来源：http://ihi.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yzc.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://gpd.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mex.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vox.shuidangran.top

Ruby: arr.sort
来源：http://kqt.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://zvp.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xyp.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lxn.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svq.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qep.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zra.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kic.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mci.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://era.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zeo.pycfn.com

[D11] 反转数组
来源：http://iez.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://xnd.ivvv.top

PHP:  array_reverse($arr);
来源：http://jzl.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dzi.zhijiandao.cn

TS:   [...arr].reverse();
来源：http://zuk.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://ahp.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://cqe.hfpthk.cn

Ruby: arr.reverse
来源：http://fcm.ppjwa.cn

C#:   list.Reverse();
来源：http://iek.yuanzhike.top

[D12] 查找元素下标
来源：http://nvq.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://cbt.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpa.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lft.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oxc.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vcd.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://vfk.zhoulong.xyz

Ruby: arr.index(x)
来源：http://hua.hcnkem.com

C#:   list.IndexOf(x);
来源：http://ppd.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://mgl.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xfx.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gmy.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://zwy.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://wki.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://omc.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ago.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hik.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qqo.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://lqy.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vow.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eva.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://cyx.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://clz.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tpj.zdbjq.cn

Go:   // 手写循环
来源：http://kff.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://czs.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mtl.gzhubu.top

[D15] 去重
来源：http://pqp.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tpe.yonumen.top

PHP:  array_unique($arr);
来源：http://tir.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://qpn.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://ddn.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gmp.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pcq.yangfankeji.com

Ruby: arr.uniq
来源：http://egx.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://vjm.ydjk.org.cn

[D16] 求和与平均值
来源：http://tzn.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fhc.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gcv.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dso.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpf.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dps.zhengqikj.top

Go:   // 手写循环累加
来源：http://dpt.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lyq.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://hrm.daria6918.cn

[D17] 最大值与最小值
来源：http://juj.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://lmu.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://eud.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pmj.bjfxy.top

TS:   Math.max(...arr);
来源：http://sqv.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bxr.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://esi.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://dxm.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://oxl.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://rfo.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hiv.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://raz.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qjk.fanxiaobao.xyz

TS:   nested.flat();
来源：http://pcu.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://khy.sjlbkw.cn

Go:   // 手写双层循环
来源：http://hln.guannengcc.top

Ruby: nested.flatten
来源：http://uhd.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uso.iojbl.cn

[D19] 按字段分组
来源：http://sqz.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fjz.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uup.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jtc.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rcv.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kik.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://lcr.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://npk.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jmn.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://vdp.xuanzx.com

Py:   Counter(arr)
来源：http://etk.xinyue.icu

PHP:  array_count_values($arr);
来源：http://ozv.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ycp.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahk.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dph.havefunace.top

Go:   // 手写 map[T]int
来源：http://dbr.gaohongyu789.top

Ruby: arr.tally
来源：http://nsg.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mkp.ydzc1.top

[D21] 判断是否包含某元素
来源：http://tei.zhixingplan.top

Py:   x in arr
来源：http://jqh.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://pol.redwolf501.top

JS:   arr.includes(x)
来源：http://rtj.jiagoushi.top

TS:   arr.includes(x)
来源：http://lly.tarul.cn

Java: list.contains(x)
来源：http://grr.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://tuy.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://cla.sweek.top

C#:   list.Contains(x)
来源：http://sza.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://yav.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://adm.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ryw.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ibu.zhaomingkeji.xyz

TS:   [...arr];
来源：http://rxi.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://igc.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hvp.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://efm.xinyue.icu

C#:   new List<int>(list);
来源：http://dss.tianlin.xyz

[D23] reduce 累积计算
来源：http://osv.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zaq.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fhk.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abm.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fey.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zvz.ydzc1.top

Go:   // 手写循环
来源：http://oxe.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ngs.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rrf.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://pwf.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ktn.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ewl.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yhg.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ibk.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fak.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yin.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kkk.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ujc.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://mzy.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nsf.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://htx.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://udi.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qyw.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ikx.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zqj.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ipw.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pez.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://wam.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://ugw.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://vyx.andypj.xyz

JS:   arr.join(", ")
来源：http://dmw.meibo888.top

TS:   arr.join(", ")
来源：http://cae.hfpthk.cn

Java: String.join(", ", list)
来源：http://dcr.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://kgz.hywenlv.cn

Ruby: arr.join(", ")
来源：http://coh.hesvh.cn

C#:   string.Join(", ", list)
来源：http://kbr.zhongyouzk.top

================================================================================
来源：http://qbe.jinghuilouyu.cn

E. 字符串处理
来源：http://bec.ybcxt.top

================================================================================
来源：http://dzo.sjlbkw.cn

[E01] 拼接字符串
来源：http://iql.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sto.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ttc.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfc.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://laa.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://voc.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://crh.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://auo.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://anu.uphjek.com

[E02] 重复字符串
来源：http://lvi.yuxming.cn

Py:   "ab" * 3
来源：http://lyz.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://bsc.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://onw.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://taw.haohaochexian.top

Java: "ab".repeat(3)
来源：http://dsw.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://qci.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://eus.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zjn.chenlongwang.top

[E03] 截取子串
来源：http://ktw.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uop.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://irr.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pns.smart0.xyz

TS:   s.slice(1, 4)
来源：http://iso.daria6918.cn

Java: s.substring(1, 4)
来源：http://ryz.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wlr.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://odp.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://lko.fktsv.cn

[E04] 查找子串位置
来源：http://otd.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://axi.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://tgu.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hiy.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://ddx.quarkkingdee.top

Java: s.indexOf("x")
来源：http://pno.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://qyu.cashguo.top

Ruby: s.index("x")
来源：http://ixi.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://mzr.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://xwm.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gwt.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ror.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tmv.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://utm.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbc.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hoz.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ktc.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cch.zhongyouzk.top


<!-- 参考信息 -->