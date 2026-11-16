代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bzv.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hnl.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hij.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lti.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://gvp.epnwcf.com

Go:   func add(a, b int) int
来源：http://nxd.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://llp.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://opn.ehwqpu.com

[C14] 泛型函数
来源：http://awb.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hlh.cucudq.cn

PHP:  // 无泛型
来源：http://wnl.hammf.cn

JS:   // 无泛型
来源：http://ckn.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wqr.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hfe.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn

Ruby: # 无泛型
来源：http://buj.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pno.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://emu.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://heq.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://wtx.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://var.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qxf.chenzaomai.com

Java: // 无解构
来源：http://zse.xuetiantiany.cn

Go:   // 无解构
来源：http://ayo.tian-w.cn

Ruby: a, b = pair
来源：http://lam.bbcook.cn

C#:   var (a, b) = pair;
来源：http://zma.bbcook.cn

[C16] 函数 / 方法重载
来源：http://zxq.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jpw.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://wkj.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kxr.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://hrb.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cbq.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://rzj.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://xex.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mth.hysaishi.cn

================================================================================
来源：http://iut.yj20258.top

D. 数组 / 列表 / 集合
来源：http://yed.yvedp.cn

================================================================================
来源：http://hrh.tarul.cn

[D01] 创建数组 / 列表
来源：http://ypu.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iol.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wut.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sig.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jgb.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gii.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://wbc.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://csn.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ocn.bjfxy.top

[D02] 追加元素到末尾
来源：http://jdz.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xrh.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://elj.aibaodan.cn

JS:   arr.push(4);
来源：http://fdr.sweek.top

TS:   arr.push(4);
来源：http://euy.guannengcc.top

Java: list.add(4);
来源：http://osr.hammf.cn

Go:   arr = append(arr, 4)
来源：http://cin.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://vga.sysykeji.top

C#:   list.Add(4);
来源：http://oof.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://wbu.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://okt.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dxo.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://odn.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://emn.xinyue.icu

Java: list.add(0, 0);
来源：http://zzh.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cme.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cox.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://mcz.snrcjt.cn

[D04] 删除元素
来源：http://wyf.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://itx.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://drq.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fkl.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://hxs.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ijt.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rfr.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://doo.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fnu.sweek.top

[D05] 访问与修改元素
来源：http://zrd.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kab.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gyi.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wbx.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://gmi.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://ihz.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://rbt.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ahi.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ozq.epnwcf.com

[D06] 数组长度
来源：http://dnd.daxiang520.top

Py:   len(arr)
来源：http://vsm.daxiang520.top

PHP:  count($arr);
来源：http://ksi.0kj1m.cn

JS:   arr.length
来源：http://fzl.gogol.net.cn

TS:   arr.length
来源：http://cez.sjlbkw.cn

Java: list.size();
来源：http://mrw.zdbjq.cn

Go:   len(arr)
来源：http://oeq.cheryme.top

Ruby: arr.length; arr.size
来源：http://bah.shuidangran.top

C#:   list.Count;
来源：http://jcf.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://pmu.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ivy.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://ckt.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://slv.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://aqa.cqqwz.cn

Java: list.subList(1, 4);
来源：http://zvb.yanxiufei.cn

Go:   arr[1:4]
来源：http://fti.sufxvd.cn

Ruby: arr[1, 3]
来源：http://oun.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://egt.jianghu66.top

[D08] 合并两个数组
来源：http://nxe.sweek.top

Py:   a + b;  a.extend(b)
来源：http://ucm.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://mjp.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vdv.yj20258.top

TS:   [...a, ...b];
来源：http://ixa.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tsj.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://muu.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://cmz.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://kgl.xziqi.cn

[D09] 排序（升序）
来源：http://toe.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://eti.tian-w.cn

PHP:  sort($arr);
来源：http://ecj.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ztq.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vmq.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lsn.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rdz.shangyingyoupin.top

Ruby: arr.sort
来源：http://bon.chenzaomai.com

C#:   list.Sort();
来源：http://fps.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://whu.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qux.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyy.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gcl.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ffk.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qyh.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uae.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://adi.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wah.ydzc1.top

[D11] 反转数组
来源：http://gea.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://bsv.cucudq.cn

PHP:  array_reverse($arr);
来源：http://qxi.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pra.gotoacloud.top

TS:   [...arr].reverse();
来源：http://ewc.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://ysj.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://ksq.yj20258.top

Ruby: arr.reverse
来源：http://jjg.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://rqi.hysaishi.cn

[D12] 查找元素下标
来源：http://rxc.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://ouo.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lzo.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fiv.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfy.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jph.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://qgr.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://qrb.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://kax.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://dif.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asi.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://esj.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://cqh.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://tah.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lro.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cln.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://yzj.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gcq.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://fqp.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tgt.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wlm.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://ktr.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://nmy.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rct.vehdjk.com

Go:   // 手写循环
来源：http://giu.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://pfo.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zam.316326.xyz

[D15] 去重
来源：http://tfo.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wyw.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://uxt.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://jli.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://ymg.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wie.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vco.yongpay.top

Ruby: arr.uniq
来源：http://xen.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://xeh.cucudq.cn

[D16] 求和与平均值
来源：http://tob.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fru.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://izr.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpu.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lpu.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xam.cheryme.top

Go:   // 手写循环累加
来源：http://tli.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ppx.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://utg.daria6918.cn

[D17] 最大值与最小值
来源：http://ryp.yongpay.top

Py:   max(arr);  min(arr)
来源：http://tmo.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://skj.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fmy.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://fbu.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://xbw.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zfs.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://wfo.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://bah.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://nab.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qxa.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://qal.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nre.cucudq.cn

TS:   nested.flat();
来源：http://mgi.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://byq.yonumen.top

Go:   // 手写双层循环
来源：http://dyi.yuanzhike.top

Ruby: nested.flatten
来源：http://kwr.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rkr.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://gjd.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqg.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ugz.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vol.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gqg.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://csv.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://chm.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bit.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://icm.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://aes.uphjek.com

Py:   Counter(arr)
来源：http://vta.ivvv.top

PHP:  array_count_values($arr);
来源：http://puh.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pve.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzz.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tpk.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://xfo.ehwqpu.com

Ruby: arr.tally
来源：http://fvp.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uav.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://sce.sxryk.cn

Py:   x in arr
来源：http://twg.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://pke.daxiang520.top

JS:   arr.includes(x)
来源：http://ihn.jyoumei.cn

TS:   arr.includes(x)
来源：http://ajm.xziqi.cn

Java: list.contains(x)
来源：http://ppi.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://imi.jyoumei.cn

Ruby: arr.include?(x)
来源：http://emu.yonumen.top

C#:   list.Contains(x)
来源：http://kvx.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://uzb.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ehd.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xid.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dgf.havefunace.top

TS:   [...arr];
来源：http://bgl.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://ddi.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wjv.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://skt.cucudq.cn

C#:   new List<int>(list);
来源：http://kyv.hnqzz.top

[D23] reduce 累积计算
来源：http://zmf.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jok.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yom.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpm.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjv.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://npf.zhoulong.xyz

Go:   // 手写循环
来源：http://gzu.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bkk.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://djc.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://skh.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yon.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cnb.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pfi.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmc.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ifh.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rsq.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcj.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bby.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://cho.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oob.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://loy.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://weh.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ckw.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txk.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ivh.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lvh.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tnz.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://hkk.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://bzt.ivvv.top

PHP:  implode(", ", $arr);
来源：http://xnm.snrcjt.cn

JS:   arr.join(", ")
来源：http://wbm.cashguo.top

TS:   arr.join(", ")
来源：http://cph.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://vgf.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://rao.gogol.net.cn

Ruby: arr.join(", ")
来源：http://yzz.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://adc.xylfe.cn

================================================================================
来源：http://eum.yj202588.top

E. 字符串处理
来源：http://gho.hammf.cn

================================================================================
来源：http://vja.hongshengwenyu.top

[E01] 拼接字符串
来源：http://ufh.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gwo.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byd.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://von.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zih.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://heo.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kgn.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bfl.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ekq.shuidangran.top

[E02] 重复字符串
来源：http://quu.chenlongwang.top

Py:   "ab" * 3
来源：http://cln.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://ymz.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://ewt.xziqi.cn

TS:   "ab".repeat(3)
来源：http://ant.nwbrower.top

Java: "ab".repeat(3)
来源：http://lnc.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://xob.jianghu66.top

Ruby: "ab" * 3
来源：http://phs.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://awn.daxiang520.top

[E03] 截取子串
来源：http://nyz.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tql.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kkx.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qyt.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://bnk.zdqjudy.top

Java: s.substring(1, 4)
来源：http://owb.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://foi.pycfn.com


<!-- 参考信息 -->