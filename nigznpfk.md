代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ego.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sdb.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://svf.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctw.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://ils.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://iwp.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sxq.bjfxy.top

[D02] 追加元素到末尾
来源：http://bvd.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxk.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://awx.chenlongwang.top

JS:   arr.push(4);
来源：http://btw.xuetiantiany.cn

TS:   arr.push(4);
来源：http://brl.zycfv.cn

Java: list.add(4);
来源：http://lzc.yonumen.top

Go:   arr = append(arr, 4)
来源：http://fkx.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://vjh.snrcjt.cn

C#:   list.Add(4);
来源：http://oob.yongpay.top

[D03] 在指定位置插入元素
来源：http://ojl.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://lmn.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nqo.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nep.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://vza.zhengqikj.top

Java: list.add(0, 0);
来源：http://kqb.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://rtn.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xmv.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://avs.c1oappe.top

[D04] 删除元素
来源：http://rkc.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iyl.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oiv.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eqg.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://tkk.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osm.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oif.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://psq.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uxo.ivvv.top

[D05] 访问与修改元素
来源：http://ldt.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmx.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yhw.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dna.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://zmh.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://yfc.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://cdf.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zbs.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mly.zhengqikj.top

[D06] 数组长度
来源：http://mfe.yj20258.top

Py:   len(arr)
来源：http://gty.zdbjq.cn

PHP:  count($arr);
来源：http://kya.xinyue.icu

JS:   arr.length
来源：http://sfb.nanxinkj.top

TS:   arr.length
来源：http://hoh.shanyushiyangkeji.top

Java: list.size();
来源：http://adu.yonumen.top

Go:   len(arr)
来源：http://zku.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://wcf.gogol.net.cn

C#:   list.Count;
来源：http://qjn.ydzc1.top

[D07] 切片 / 取子数组
来源：http://mgk.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rte.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yoq.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://qoy.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://sjz.aizwys.cn

Java: list.subList(1, 4);
来源：http://oca.52xcode.cn

Go:   arr[1:4]
来源：http://wdx.c1oappe.top

Ruby: arr[1, 3]
来源：http://yac.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://zod.dianchejie.cn

[D08] 合并两个数组
来源：http://avy.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://lro.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://dpn.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://snc.zhixingplan.top

TS:   [...a, ...b];
来源：http://iib.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qyh.vehdjk.com

Go:   append(a, b...)
来源：http://byz.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://mua.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://buo.yj20258.top

[D09] 排序（升序）
来源：http://url.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://qcv.ppjwa.cn

PHP:  sort($arr);
来源：http://gsw.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qal.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yhm.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zsx.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uja.fzhhl.top

Ruby: arr.sort
来源：http://eya.shuidangran.top

C#:   list.Sort();
来源：http://ute.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jza.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://avp.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://evz.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://far.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jow.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kcq.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wml.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gwe.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tzi.ppjwa.cn

[D11] 反转数组
来源：http://tbs.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iwe.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://qoe.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://anb.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://gde.316326.xyz

Java: Collections.reverse(list);
来源：http://uyi.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://dqz.cashguo.top

Ruby: arr.reverse
来源：http://ehs.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://dsm.zdbjq.cn

[D12] 查找元素下标
来源：http://gad.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://sir.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uva.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ads.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjk.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vfj.ivvv.top

Go:   slices.Index(arr, x)
来源：http://sdt.yvedp.cn

Ruby: arr.index(x)
来源：http://etv.pycfn.com

C#:   list.IndexOf(x);
来源：http://viv.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://cvc.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nrr.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hlm.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://mrx.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://ohs.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oad.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flw.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://ekr.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ppm.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://kco.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://abi.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://suq.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://stw.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://djy.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yeh.andypj.xyz

Go:   // 手写循环
来源：http://chm.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://whh.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fbd.epnwcf.com

[D15] 去重
来源：http://eng.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqz.shuidangran.top

PHP:  array_unique($arr);
来源：http://sty.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://oax.sweek.top

TS:   [...new Set(arr)]
来源：http://gbd.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gtv.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pon.shzxlz.cn

Ruby: arr.uniq
来源：http://aum.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://vvr.sufxvd.cn

[D16] 求和与平均值
来源：http://bmt.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bra.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tdt.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kyh.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bks.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ggo.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://bge.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gmq.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://kll.zhijiandao.cn

[D17] 最大值与最小值
来源：http://cky.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://omd.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://lac.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vxl.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://gox.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tir.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lhw.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://rmm.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://lnm.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://dzy.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vtx.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://jof.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zyd.hnqzz.top

TS:   nested.flat();
来源：http://ysy.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arm.smart0.xyz

Go:   // 手写双层循环
来源：http://rzk.jlsjyb.cn

Ruby: nested.flatten
来源：http://kpq.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ati.zycfv.cn

[D19] 按字段分组
来源：http://kgd.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsz.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vvt.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jut.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vtp.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ded.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://nmn.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wim.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gos.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://vvl.ehwqpu.com

Py:   Counter(arr)
来源：http://hhw.yj202588.top

PHP:  array_count_values($arr);
来源：http://jnd.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ysh.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mwp.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iry.meibo888.top

Go:   // 手写 map[T]int
来源：http://mbz.cashguo.top

Ruby: arr.tally
来源：http://xtd.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yco.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://gwx.snrcjt.cn

Py:   x in arr
来源：http://idu.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://rqs.meibo888.top

JS:   arr.includes(x)
来源：http://wwd.jiagoushi.top

TS:   arr.includes(x)
来源：http://elb.chenjidiqi.icu

Java: list.contains(x)
来源：http://vhc.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://dbi.xylfe.cn

Ruby: arr.include?(x)
来源：http://hfm.chenlongwang.top

C#:   list.Contains(x)
来源：http://zyr.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://ijh.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwi.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ros.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ozr.xuetiantiany.cn

TS:   [...arr];
来源：http://ciu.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://ovt.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xxy.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://zhz.gaohongyu789.top

C#:   new List<int>(list);
来源：http://wsv.cdnleiting.top

[D23] reduce 累积计算
来源：http://clc.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aly.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kee.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywt.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cbh.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://xdn.hnxiangtu.top

Go:   // 手写循环
来源：http://ovb.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ppb.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvc.sweek.top

[D24] 字典 / Map 基本操作
来源：http://qbg.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://esh.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lur.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hvr.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://twn.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fwa.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://auc.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nqe.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qpo.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://eeu.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzb.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://atc.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rqs.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gsu.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://guj.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xsn.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fkz.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zpj.tanke756.top

[D26] 数组转字符串
来源：http://dze.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://fhh.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://dhw.epnwcf.com

JS:   arr.join(", ")
来源：http://paj.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://dtl.yj202588.top

Java: String.join(", ", list)
来源：http://nsb.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://fym.sxryk.cn

Ruby: arr.join(", ")
来源：http://kmj.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://gyp.sysykeji.top

================================================================================
来源：http://eiw.bjfxy.top

E. 字符串处理
来源：http://qno.dashuyun.cn

================================================================================
来源：http://amk.sjlbkw.cn

[E01] 拼接字符串
来源：http://rte.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pzu.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uil.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqy.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zue.hfpthk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mvm.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kwp.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kmy.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://frk.hesvh.cn

[E02] 重复字符串
来源：http://ybh.ydzc1.top

Py:   "ab" * 3
来源：http://gzf.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://qsu.52xcode.cn

JS:   "ab".repeat(3)
来源：http://srx.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://vmc.yj20258.top

Java: "ab".repeat(3)
来源：http://tut.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://lss.hywenlv.cn

Ruby: "ab" * 3
来源：http://iql.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cnx.jqgfzy.top

[E03] 截取子串
来源：http://ulq.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xbi.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vnt.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pqf.ivvv.top

TS:   s.slice(1, 4)
来源：http://dtd.yj202588.top

Java: s.substring(1, 4)
来源：http://odt.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yjn.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://smx.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://yid.redwolf501.top

[E04] 查找子串位置
来源：http://kwx.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://soh.fzhhl.top

PHP:  strpos($s, "x");
来源：http://uzh.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://leq.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://tzp.ehwqpu.com

Java: s.indexOf("x")
来源：http://vse.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://iew.bjfxy.top

Ruby: s.index("x")
来源：http://kuz.yvedp.cn

C#:   s.IndexOf("x")
来源：http://spe.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nlp.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nid.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://and.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jbf.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://azi.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsl.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ztt.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uta.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fuf.9152youxi.cn

[E06] 替换子串
来源：http://uro.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://orr.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://eok.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nkw.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://beh.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oyk.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rld.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xbx.tarul.cn

C#:   s.Replace("a", "b")
来源：http://klq.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://hsz.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzf.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ihs.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kcc.daria6918.cn

TS:   s.split(",")
来源：http://lvq.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://mwj.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lul.tanke756.top

Ruby: s.split(",");  s.split
来源：http://bso.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://imj.316326.xyz

[E08] 数组按分隔符合并
来源：http://jxr.cqqwz.cn

Py:   ",".join(items)
来源：http://ytp.zhongyouzk.top


<!-- 参考信息 -->