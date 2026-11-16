代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nud.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wlz.zhiwuduotai.top

Java: // 无解构
来源：http://ziz.tianlin.xyz

Go:   // 无解构
来源：http://gqn.fehbvm.com

Ruby: a, b = pair
来源：http://duj.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://qfv.fehbvm.com

[C16] 函数 / 方法重载
来源：http://ebs.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mqo.sxryk.cn

PHP:  // 无重载
来源：http://exh.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qga.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://uck.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rbo.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://poa.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://dib.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://uny.iojbl.cn

================================================================================
来源：http://xxe.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://htm.ydjk.org.cn

================================================================================
来源：http://lbu.yj202588.top

[D01] 创建数组 / 列表
来源：http://ljf.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kab.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pde.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wfb.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ulj.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dhh.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://itu.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://gpw.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tox.yuanzhike.top

[D02] 追加元素到末尾
来源：http://csh.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bee.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xsr.zycfv.cn

JS:   arr.push(4);
来源：http://ruy.hnxiangtu.top

TS:   arr.push(4);
来源：http://dlp.chenjidiqi.icu

Java: list.add(4);
来源：http://fdv.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://nfq.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://yvq.chenlongwang.top

C#:   list.Add(4);
来源：http://joh.sxryk.cn

[D03] 在指定位置插入元素
来源：http://jkh.tanke756.top

Py:   arr.insert(0, 0)
来源：http://jno.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rws.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fbe.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://hre.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://boe.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://gar.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qmj.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://sez.zhijiandao.cn

[D04] 删除元素
来源：http://sqq.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oad.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hzi.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mmx.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://agd.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fue.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qpb.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lwl.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sow.yj20258888.top

[D05] 访问与修改元素
来源：http://tlz.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xsn.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uif.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zcq.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://kfi.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://vqb.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://nil.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yoa.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cxm.zhixingplan.top

[D06] 数组长度
来源：http://ixn.haohaochexian.top

Py:   len(arr)
来源：http://gav.jinqigufen.top

PHP:  count($arr);
来源：http://qnm.xylfe.cn

JS:   arr.length
来源：http://wvu.ivvv.top

TS:   arr.length
来源：http://bdx.jinyuanbaomall.cn

Java: list.size();
来源：http://rji.c1oappe.top

Go:   len(arr)
来源：http://ehd.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://cxe.zhoulong.xyz

C#:   list.Count;
来源：http://apk.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://psc.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mty.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ejy.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://fdf.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://afo.tarul.cn

Java: list.subList(1, 4);
来源：http://jec.tianlin.xyz

Go:   arr[1:4]
来源：http://kvh.shuidangran.top

Ruby: arr[1, 3]
来源：http://mig.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://iqe.hammf.cn

[D08] 合并两个数组
来源：http://nwl.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://utg.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://any.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wsm.bbcook.cn

TS:   [...a, ...b];
来源：http://hox.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lxl.meibo888.top

Go:   append(a, b...)
来源：http://izm.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://els.0kj1m.cn

C#:   a.Concat(b).ToList()
来源：http://shl.shzxlz.cn

[D09] 排序（升序）
来源：http://uik.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://kcb.xinyue.icu

PHP:  sort($arr);
来源：http://pcm.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fgs.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wof.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bdt.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tbf.yuxming.cn

Ruby: arr.sort
来源：http://efd.sweek.top

C#:   list.Sort();
来源：http://sny.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjk.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://huz.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eek.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhr.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqb.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oyk.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rhe.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://czp.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jre.dashuyun.cn

[D11] 反转数组
来源：http://iup.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://bky.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://syj.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ewo.jyoumei.cn

TS:   [...arr].reverse();
来源：http://ibs.hnqzz.top

Java: Collections.reverse(list);
来源：http://kyw.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://npl.tian-w.cn

Ruby: arr.reverse
来源：http://oyl.zhongyouzk.top

C#:   list.Reverse();
来源：http://jqx.jyoumei.cn

[D12] 查找元素下标
来源：http://zvw.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://mxo.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lvl.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vmm.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://odk.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njv.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://mpa.9152youxi.cn

Ruby: arr.index(x)
来源：http://kuc.c1oappe.top

C#:   list.IndexOf(x);
来源：http://hzk.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://uvc.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jkw.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zvx.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://xnf.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://jrn.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yfj.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lzh.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fsz.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://npn.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://eha.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fch.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iqf.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://mkx.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://iba.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kjh.quarkkingdee.top

Go:   // 手写循环
来源：http://ufn.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sga.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pdl.cucudq.cn

[D15] 去重
来源：http://bjp.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://azi.meibo888.top

PHP:  array_unique($arr);
来源：http://bwe.yj202588.top

JS:   [...new Set(arr)]
来源：http://tnh.cucudq.cn

TS:   [...new Set(arr)]
来源：http://cvp.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ipt.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://dpt.ppjwa.cn

Ruby: arr.uniq
来源：http://rsv.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://ehe.nanxinkj.top

[D16] 求和与平均值
来源：http://npj.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rrp.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rlm.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://niz.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://agp.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rui.birdmap.top

Go:   // 手写循环累加
来源：http://aml.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://njb.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://unt.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://oac.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://and.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://kgw.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xum.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://bny.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://faz.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://otf.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://ynv.yongpay.top

C#:   list.Max();  list.Min()
来源：http://bxi.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://jdy.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hrx.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://iwc.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ghx.zhengqikj.top

TS:   nested.flat();
来源：http://kfd.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kst.hnqzz.top

Go:   // 手写双层循环
来源：http://bip.hnqzz.top

Ruby: nested.flatten
来源：http://ypy.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xyd.snrcjt.cn

[D19] 按字段分组
来源：http://gsc.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gzc.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddq.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iob.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsh.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ips.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://mwp.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://esp.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rre.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://lva.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://sca.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://frt.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cif.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xdb.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dup.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://ybm.316326.xyz

Ruby: arr.tally
来源：http://ibw.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fwf.fktsv.cn

[D21] 判断是否包含某元素
来源：http://bks.hcnkem.com

Py:   x in arr
来源：http://dkf.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://tei.nanxinkj.top

JS:   arr.includes(x)
来源：http://jnk.zdqjudy.top

TS:   arr.includes(x)
来源：http://vpe.0kj1m.cn

Java: list.contains(x)
来源：http://kmt.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://mvh.ehwqpu.com

Ruby: arr.include?(x)
来源：http://pez.hnxiangtu.top

C#:   list.Contains(x)
来源：http://usn.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://dur.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://goq.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uxg.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jbd.shuidangran.top

TS:   [...arr];
来源：http://trv.hesvh.cn

Java: new ArrayList<>(list);
来源：http://ptw.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://ydp.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://ltz.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://mwr.sufxvd.cn

[D23] reduce 累积计算
来源：http://myt.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zzf.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qgq.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://apb.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xuv.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ghj.xylfe.cn

Go:   // 手写循环
来源：http://pxh.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://utp.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://slu.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://wmf.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gdl.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yjw.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tbr.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fop.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ebf.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ghb.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mng.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://msm.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://qav.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hff.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jsx.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aeg.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oas.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pts.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mbn.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nba.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rca.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://kvw.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://bmy.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://yxu.jinqigufen.top

JS:   arr.join(", ")
来源：http://yrj.jqgfzy.top

TS:   arr.join(", ")
来源：http://hak.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://djw.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://sox.aizwys.cn

Ruby: arr.join(", ")
来源：http://int.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://bra.ydjk.org.cn

================================================================================
来源：http://kni.chenjidiqi.icu

E. 字符串处理
来源：http://gtr.sjlbkw.cn

================================================================================
来源：http://fhs.aibaodan.cn

[E01] 拼接字符串
来源：http://mco.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://crz.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lzf.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://idd.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nlx.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jux.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dwa.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mqi.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kde.chenzaomai.com

[E02] 重复字符串
来源：http://igp.hnxiangtu.top

Py:   "ab" * 3
来源：http://jrn.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://rha.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://zkc.cucudq.cn

TS:   "ab".repeat(3)
来源：http://wmj.9152youxi.cn

Java: "ab".repeat(3)
来源：http://kdc.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://avb.ydjk.org.cn

Ruby: "ab" * 3
来源：http://syf.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://euj.redwolf501.top

[E03] 截取子串
来源：http://fhg.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ere.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ozd.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dje.uphjek.com

TS:   s.slice(1, 4)
来源：http://uqd.yj20258888.top

Java: s.substring(1, 4)
来源：http://hku.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yaw.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://kfc.yonumen.top

C#:   s.Substring(1, 3)
来源：http://maq.jyoumei.cn

[E04] 查找子串位置
来源：http://fce.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://gtg.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://obn.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hdj.uphjek.com

TS:   s.indexOf("x")
来源：http://dzz.jinqigfzy.top

Java: s.indexOf("x")
来源：http://uvu.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://gqu.xylfe.cn

Ruby: s.index("x")
来源：http://zjw.ybcxt.top

C#:   s.IndexOf("x")
来源：http://znz.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vyy.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sov.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ofy.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzt.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfv.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kmy.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nzs.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bfp.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wdc.nanxinkj.top


<!-- 参考信息 -->