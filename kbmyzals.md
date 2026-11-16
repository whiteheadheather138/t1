代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zgh.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cdb.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nrj.quarkkingdee.top

Ruby: # 无泛型
来源：http://xwk.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rzl.havefunace.top

[C15] 解构 / 展开参数
来源：http://hiq.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cdi.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://foq.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yiq.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fcg.snrcjt.cn

Java: // 无解构
来源：http://vib.mhx1999.top

Go:   // 无解构
来源：http://clk.yj202588.top

Ruby: a, b = pair
来源：http://xne.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://fxt.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://jre.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wrr.haohaochexian.top

PHP:  // 无重载
来源：http://iiz.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vvi.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://ald.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://htk.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://rvc.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://ujz.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gsr.gogol.net.cn

================================================================================
来源：http://yzt.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://cxs.nwbrower.top

================================================================================
来源：http://nzr.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://lrs.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ayl.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qnx.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jnz.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lzg.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vpc.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://dzg.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://qbt.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mec.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://ljb.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://huj.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://atl.jqgufenzy.top

JS:   arr.push(4);
来源：http://pkw.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://ped.dianchejie.cn

Java: list.add(4);
来源：http://qiy.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://qzd.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://nve.snrcjt.cn

C#:   list.Add(4);
来源：http://sci.hammf.cn

[D03] 在指定位置插入元素
来源：http://dwp.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://rmd.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cdd.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ytv.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://njb.vehdjk.com

Java: list.add(0, 0);
来源：http://drd.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://kev.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kbq.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://qpj.shanyushiyangkeji.top

[D04] 删除元素
来源：http://oml.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wyn.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://drz.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zce.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://ljp.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mal.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cbe.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rss.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ezj.jiagoushi.top

[D05] 访问与修改元素
来源：http://gal.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dkv.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://onp.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zfs.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://vmx.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://rcy.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ter.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rvf.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xte.52xcode.cn

[D06] 数组长度
来源：http://dvu.shzxlz.cn

Py:   len(arr)
来源：http://unv.fktsv.cn

PHP:  count($arr);
来源：http://tqb.316326.xyz

JS:   arr.length
来源：http://mbl.fehbvm.com

TS:   arr.length
来源：http://hgs.daria6918.cn

Java: list.size();
来源：http://njm.smart0.xyz

Go:   len(arr)
来源：http://eni.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://nzr.birdmap.top

C#:   list.Count;
来源：http://lxt.cashguo.top

[D07] 切片 / 取子数组
来源：http://kqo.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whm.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uem.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://fbp.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://vws.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://hrs.nwbrower.top

Go:   arr[1:4]
来源：http://fgp.jiagoushi.top

Ruby: arr[1, 3]
来源：http://rfk.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://gpf.cashguo.top

[D08] 合并两个数组
来源：http://lrb.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://xhr.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://hox.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://hib.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://xsy.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cya.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://zzh.gotoacloud.top

Ruby: a + b;  a.concat(b)
来源：http://zdt.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://epf.epnwcf.com

[D09] 排序（升序）
来源：http://fex.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://oof.tianlin.xyz

PHP:  sort($arr);
来源：http://fym.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://asl.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cna.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jxm.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kpj.zdqjudy.top

Ruby: arr.sort
来源：http://dlx.ctjpmb.com

C#:   list.Sort();
来源：http://fng.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xei.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ncu.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dgy.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmw.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgn.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yjt.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vnc.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vda.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oid.havefunace.top

[D11] 反转数组
来源：http://iis.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xwp.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://sni.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uus.fengsongda.top

TS:   [...arr].reverse();
来源：http://ior.sufxvd.cn

Java: Collections.reverse(list);
来源：http://wke.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://rqb.hnqzz.top

Ruby: arr.reverse
来源：http://rht.jinqigfzy.top

C#:   list.Reverse();
来源：http://qst.cqqwz.cn

[D12] 查找元素下标
来源：http://nkz.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://rfy.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qit.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twz.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ytp.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nvd.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://wjh.smart0.xyz

Ruby: arr.index(x)
来源：http://hgz.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://yey.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://vof.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://azl.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://glg.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://tuy.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://buy.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dgx.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dhl.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://jnc.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://gks.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://ewm.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oap.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oce.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://xry.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://jqf.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://spc.epnwcf.com

Go:   // 手写循环
来源：http://qnz.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xqu.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hxc.fengsongda.top

[D15] 去重
来源：http://lhr.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kon.xuanzx.com

PHP:  array_unique($arr);
来源：http://uik.sysykeji.top

JS:   [...new Set(arr)]
来源：http://bkc.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://bcy.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rwd.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xhv.zycfv.cn

Ruby: arr.uniq
来源：http://fvb.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://bos.bjfxy.top

[D16] 求和与平均值
来源：http://ygl.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tex.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ovm.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ndf.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://doa.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kzx.sweek.top

Go:   // 手写循环累加
来源：http://vdd.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ezm.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://zkn.ehwqpu.com

[D17] 最大值与最小值
来源：http://glg.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://ifv.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://sdm.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://huo.cashguo.top

TS:   Math.max(...arr);
来源：http://olj.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qdd.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pmj.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://poo.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://tmy.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://oll.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wzh.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://ihm.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vek.daxiang520.top

TS:   nested.flat();
来源：http://wov.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dtu.yangfankeji.com

Go:   // 手写双层循环
来源：http://hhs.jiagoushi.top

Ruby: nested.flatten
来源：http://pyb.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://exu.hnxiangtu.top

[D19] 按字段分组
来源：http://qps.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mag.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tlj.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ihi.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://koz.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dad.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://had.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://loe.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zti.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://mrh.cucudq.cn

Py:   Counter(arr)
来源：http://cxn.bjfxy.top

PHP:  array_count_values($arr);
来源：http://wsu.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uhb.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwg.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zrv.316326.xyz

Go:   // 手写 map[T]int
来源：http://xqb.hesvh.cn

Ruby: arr.tally
来源：http://wgq.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ado.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://owx.ydzc1.top

Py:   x in arr
来源：http://sxq.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://rdj.fengsongda.top

JS:   arr.includes(x)
来源：http://hph.hnxiangtu.top

TS:   arr.includes(x)
来源：http://ldq.tianlin.xyz

Java: list.contains(x)
来源：http://yua.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://eii.tarul.cn

Ruby: arr.include?(x)
来源：http://nbf.xuanzx.com

C#:   list.Contains(x)
来源：http://pzw.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://wqz.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://idz.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bab.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zye.yanxiufei.cn

TS:   [...arr];
来源：http://czp.ivvv.top

Java: new ArrayList<>(list);
来源：http://uuo.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://mrs.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://gta.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://htw.tian-w.cn

[D23] reduce 累积计算
来源：http://ava.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vki.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hgl.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgh.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fqq.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tlj.sysykeji.top

Go:   // 手写循环
来源：http://hkr.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxe.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://btl.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://jwh.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xjy.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bwg.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gmc.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kcl.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zyc.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hdi.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bpi.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wcf.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://xud.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dop.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qwk.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yiv.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://prx.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qmd.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ccj.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hwi.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qnp.andypj.xyz

[D26] 数组转字符串
来源：http://hhw.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://ayb.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://ies.cashguo.top

JS:   arr.join(", ")
来源：http://bha.gotoacloud.top

TS:   arr.join(", ")
来源：http://jer.nanxuanxn.top

Java: String.join(", ", list)
来源：http://ega.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://zbf.gogol.net.cn

Ruby: arr.join(", ")
来源：http://mtc.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://rxz.shangyingyoupin.top

================================================================================
来源：http://eig.cqqwz.cn

E. 字符串处理
来源：http://jnr.chenjidiqi.icu

================================================================================
来源：http://nak.guowangkeji.top

[E01] 拼接字符串
来源：http://oqf.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ezr.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jad.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxc.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://neo.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xbm.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hoi.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hhc.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nvy.sufxvd.cn

[E02] 重复字符串
来源：http://xtd.nanxinkj.top

Py:   "ab" * 3
来源：http://bxr.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://cex.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://tlr.xuanzx.com

TS:   "ab".repeat(3)
来源：http://ctn.gotoacloud.top

Java: "ab".repeat(3)
来源：http://ukw.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://uuf.jqgufenzy.top

Ruby: "ab" * 3
来源：http://udx.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yts.jqgfzy.top

[E03] 截取子串
来源：http://eng.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ccv.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://znw.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxf.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://hqr.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://khx.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eup.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://vfk.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://eeu.gaohongyu789.top

[E04] 查找子串位置
来源：http://hky.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://yhp.hcnkem.com

PHP:  strpos($s, "x");
来源：http://fzd.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jfh.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://tia.sweek.top

Java: s.indexOf("x")
来源：http://eht.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://lvn.zdbjq.cn

Ruby: s.index("x")
来源：http://jyp.hesvh.cn

C#:   s.IndexOf("x")
来源：http://vdo.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ejm.zdbjq.cn


<!-- 参考信息 -->