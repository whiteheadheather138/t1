代发 wailian999

Ruby: a, b = pair
来源：http://irp.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://ofx.mhx1999.top

[C16] 函数 / 方法重载
来源：http://qcb.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ftv.yvedp.cn

PHP:  // 无重载
来源：http://mxo.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ysl.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://tpm.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vbd.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://ahk.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://ocm.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://fzi.epnwcf.com

================================================================================
来源：http://vxv.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://aym.vqdsnc.cn

================================================================================
来源：http://myv.ybcxt.top

[D01] 创建数组 / 列表
来源：http://are.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hzk.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fga.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ecv.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dke.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qkf.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://mvu.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://kvw.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cft.birdmap.top

[D02] 追加元素到末尾
来源：http://lpu.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://puy.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbm.gotoacloud.top

JS:   arr.push(4);
来源：http://fzy.fktsv.cn

TS:   arr.push(4);
来源：http://pqf.cqqwz.cn

Java: list.add(4);
来源：http://fqn.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://nda.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://ymf.gotoacloud.top

C#:   list.Add(4);
来源：http://pot.pycfn.com

[D03] 在指定位置插入元素
来源：http://fzi.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://iuc.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rtb.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tje.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://tuq.yangfankeji.com

Java: list.add(0, 0);
来源：http://ext.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://mwo.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ind.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://rgx.gotoacloud.top

[D04] 删除元素
来源：http://pqt.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bix.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vfl.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://thp.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://xzd.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ukm.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kmo.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vom.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nvm.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://jew.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zzi.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uwu.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vea.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://qln.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://nak.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://igw.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://shp.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xda.sxryk.cn

[D06] 数组长度
来源：http://sql.epnwcf.com

Py:   len(arr)
来源：http://gqe.yueranfly.top

PHP:  count($arr);
来源：http://rcd.9152youxi.cn

JS:   arr.length
来源：http://hma.bbcook.cn

TS:   arr.length
来源：http://qro.nanxinkj.top

Java: list.size();
来源：http://bvi.sweek.top

Go:   len(arr)
来源：http://lbq.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://ofo.wangshuangyany.cn

C#:   list.Count;
来源：http://oas.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://prh.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uas.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ftr.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://fcw.tarul.cn

TS:   arr.slice(1, 4);
来源：http://bot.ivvv.top

Java: list.subList(1, 4);
来源：http://wbf.hysaishi.cn

Go:   arr[1:4]
来源：http://ksp.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://wqw.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://zmb.yongpay.top

[D08] 合并两个数组
来源：http://iwk.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://ijm.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://krg.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://awo.sufxvd.cn

TS:   [...a, ...b];
来源：http://yrh.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://poz.chenlongwang.top

Go:   append(a, b...)
来源：http://cpw.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://jzq.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://uly.hysaishi.cn

[D09] 排序（升序）
来源：http://vaj.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://vlm.jianghu66.top

PHP:  sort($arr);
来源：http://lnw.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jqn.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rxw.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ysi.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://igi.hammf.cn

Ruby: arr.sort
来源：http://xos.cqqwz.cn

C#:   list.Sort();
来源：http://bie.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://czo.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vvi.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqo.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzk.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://shr.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bzq.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fdx.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bhe.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eqn.ctjpmb.com

[D11] 反转数组
来源：http://bks.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ysw.yj20258888.top

PHP:  array_reverse($arr);
来源：http://zdi.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yol.yonumen.top

TS:   [...arr].reverse();
来源：http://bjd.tanke756.top

Java: Collections.reverse(list);
来源：http://fmt.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://xyk.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://rci.pengpengdd.cyou

C#:   list.Reverse();
来源：http://jxs.nanxuanxn.top

[D12] 查找元素下标
来源：http://lbt.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://dzx.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ndz.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrf.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djf.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qsm.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://lgo.hnxiangtu.top

Ruby: arr.index(x)
来源：http://jai.cashguo.top

C#:   list.IndexOf(x);
来源：http://iwt.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://qbg.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lkz.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yza.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://dbq.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://eiu.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lop.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ixe.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://xzg.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lef.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://lkp.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cxq.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nvb.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://qup.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://heq.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sdi.tanke756.top

Go:   // 手写循环
来源：http://vyr.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://lok.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tic.birdmap.top

[D15] 去重
来源：http://tqy.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kpa.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://xjt.wangdashe.top

JS:   [...new Set(arr)]
来源：http://qsb.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://rfv.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cos.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gyx.fehbvm.com

Ruby: arr.uniq
来源：http://gwz.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://smw.fktsv.cn

[D16] 求和与平均值
来源：http://ddw.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://inl.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jnu.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ieb.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://awj.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bge.cdnleiting.top

Go:   // 手写循环累加
来源：http://yix.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mbe.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://czn.zycfv.cn

[D17] 最大值与最小值
来源：http://mqj.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://wpd.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://uhz.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://snm.xuanzx.com

TS:   Math.max(...arr);
来源：http://eij.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bvb.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dis.birdmap.top

Ruby: arr.max;  arr.min
来源：http://plb.uphjek.com

C#:   list.Max();  list.Min()
来源：http://toc.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://vae.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wvc.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://fib.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sqt.yj20258888.top

TS:   nested.flat();
来源：http://jjr.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zcm.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://ayy.chenlongwang.top

Ruby: nested.flatten
来源：http://enn.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lub.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://aab.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://foi.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mdl.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://agr.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rsr.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wju.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://vxg.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sik.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://spn.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://ixt.yanxiufei.cn

Py:   Counter(arr)
来源：http://yhe.hcnkem.com

PHP:  array_count_values($arr);
来源：http://vsi.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://krx.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gds.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://csh.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://qhz.zdbjq.cn

Ruby: arr.tally
来源：http://ylj.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://elf.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://yco.yuanzhike.top

Py:   x in arr
来源：http://hme.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://ljw.xylfe.cn

JS:   arr.includes(x)
来源：http://mbn.jqgfzy.top

TS:   arr.includes(x)
来源：http://qlf.sufxvd.cn

Java: list.contains(x)
来源：http://cvy.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://fqx.jinqigufen.top

Ruby: arr.include?(x)
来源：http://eqm.mhx1999.top

C#:   list.Contains(x)
来源：http://qoy.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://okz.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfy.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://emv.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ell.hfpthk.cn

TS:   [...arr];
来源：http://qbm.tarul.cn

Java: new ArrayList<>(list);
来源：http://seo.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://vfp.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://miq.zhoulong.xyz

C#:   new List<int>(list);
来源：http://lpm.chenzaomai.com

[D23] reduce 累积计算
来源：http://yth.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fuy.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nys.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://etj.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://owf.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kit.hesvh.cn

Go:   // 手写循环
来源：http://uqw.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mxq.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ycf.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://tgj.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zad.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ksm.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fdi.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ljn.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oio.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ppq.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aea.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wks.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://thr.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lof.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qkn.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://phf.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dkq.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wdr.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://emm.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ggk.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://muv.yj20258888.top

[D26] 数组转字符串
来源：http://lcg.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://jmq.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://xxl.jyoumei.cn

JS:   arr.join(", ")
来源：http://qfa.jqgufenzy.top

TS:   arr.join(", ")
来源：http://unt.guowangkeji.top

Java: String.join(", ", list)
来源：http://cdw.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://pha.bbcook.cn

Ruby: arr.join(", ")
来源：http://hbm.wangdashe.top

C#:   string.Join(", ", list)
来源：http://swr.yueranfly.top

================================================================================
来源：http://smp.fengsongda.top

E. 字符串处理
来源：http://cgk.yongpay.top

================================================================================
来源：http://yju.zycfv.cn

[E01] 拼接字符串
来源：http://bti.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://umv.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sju.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lce.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uum.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oyj.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://joe.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zxu.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://amm.zycfv.cn

[E02] 重复字符串
来源：http://ccb.snrcjt.cn

Py:   "ab" * 3
来源：http://def.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://uzx.fktsv.cn

JS:   "ab".repeat(3)
来源：http://vle.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://gfi.cashguo.top

Java: "ab".repeat(3)
来源：http://hla.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://nrn.jinqigfzy.top

Ruby: "ab" * 3
来源：http://pvl.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ufc.jinyuanbaomall.cn

[E03] 截取子串
来源：http://jaq.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dac.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwk.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://krj.xinyue.icu

TS:   s.slice(1, 4)
来源：http://lpz.mhx1999.top

Java: s.substring(1, 4)
来源：http://wpo.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://syj.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://xxn.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://xff.guannengcc.top

[E04] 查找子串位置
来源：http://aul.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://ccm.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://qwz.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://deo.fzhhl.top

TS:   s.indexOf("x")
来源：http://hie.guowangkeji.top

Java: s.indexOf("x")
来源：http://zyb.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://cof.jqgufenzy.top

Ruby: s.index("x")
来源：http://qxi.yuxming.cn

C#:   s.IndexOf("x")
来源：http://blw.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bah.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mum.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vcp.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twu.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xgz.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jof.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ffm.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ior.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ulo.daria6918.cn

[E06] 替换子串
来源：http://tkf.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://did.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://ykx.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjg.smart0.xyz


<!-- 参考信息 -->