代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dry.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjt.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xvo.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jaa.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://euf.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://iqh.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlv.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://obx.zhiwuduotai.top

[C14] 泛型函数
来源：http://nmc.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://azh.yuanzhike.top

PHP:  // 无泛型
来源：http://com.cheryme.top

JS:   // 无泛型
来源：http://yes.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://owa.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zti.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ztz.guowangkeji.top

Ruby: # 无泛型
来源：http://aab.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ibu.hammf.cn

[C15] 解构 / 展开参数
来源：http://lse.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xve.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://nvw.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://owe.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qph.feifeiyinyue.top

Java: // 无解构
来源：http://sqp.yj20258888.top

Go:   // 无解构
来源：http://coh.yonumen.top

Ruby: a, b = pair
来源：http://cyy.cucudq.cn

C#:   var (a, b) = pair;
来源：http://mhu.ivvv.top

[C16] 函数 / 方法重载
来源：http://zul.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pcz.zdqjudy.top

PHP:  // 无重载
来源：http://zta.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cpd.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://zzi.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aqv.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://vnh.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://gjm.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://urw.zhoulong.xyz

================================================================================
来源：http://qbu.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://hcr.haohaochexian.top

================================================================================
来源：http://moy.wangdashe.top

[D01] 创建数组 / 列表
来源：http://rud.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://djd.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sfm.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rll.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gmi.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://krs.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://czs.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://bax.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vsk.birdmap.top

[D02] 追加元素到末尾
来源：http://rdu.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wor.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxu.yonumen.top

JS:   arr.push(4);
来源：http://vco.hnxiangtu.top

TS:   arr.push(4);
来源：http://iqq.havefunace.top

Java: list.add(4);
来源：http://goz.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://jah.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://dfq.meibo888.top

C#:   list.Add(4);
来源：http://pho.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://flj.yj202588.top

Py:   arr.insert(0, 0)
来源：http://kwi.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cym.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dfd.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://rke.chenzaomai.com

Java: list.add(0, 0);
来源：http://lbm.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wqa.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gjy.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://orh.ivvv.top

[D04] 删除元素
来源：http://mib.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jae.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sbw.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zgc.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://alk.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zcg.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hcc.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eru.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vtb.yfazqb.com

[D05] 访问与修改元素
来源：http://uag.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dxn.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nlo.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bpm.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://jwt.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://wlu.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://qgv.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ver.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xwl.jinqigufen.top

[D06] 数组长度
来源：http://zcx.fehbvm.com

Py:   len(arr)
来源：http://rul.cdnleiting.top

PHP:  count($arr);
来源：http://uef.mhx1999.top

JS:   arr.length
来源：http://lty.havefunace.top

TS:   arr.length
来源：http://sqi.epnwcf.com

Java: list.size();
来源：http://qfg.jinqigfzy.top

Go:   len(arr)
来源：http://ifb.ivvv.top

Ruby: arr.length; arr.size
来源：http://yns.ivvv.top

C#:   list.Count;
来源：http://qde.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://pww.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fga.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://sag.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://uap.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://dxp.fengsongda.top

Java: list.subList(1, 4);
来源：http://tqa.nanxinkj.top

Go:   arr[1:4]
来源：http://idk.ppjwa.cn

Ruby: arr[1, 3]
来源：http://oci.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://ypb.zhoulong.xyz

[D08] 合并两个数组
来源：http://iiv.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://ugy.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://hph.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uqc.aibaodan.cn

TS:   [...a, ...b];
来源：http://byp.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rfr.hcnkem.com

Go:   append(a, b...)
来源：http://hiy.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://vna.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://uiu.hcnkem.com

[D09] 排序（升序）
来源：http://ccf.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://byt.shangyingyoupin.top

PHP:  sort($arr);
来源：http://waf.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bez.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://myl.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://ryv.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jjr.cashguo.top

Ruby: arr.sort
来源：http://mlc.yuxming.cn

C#:   list.Sort();
来源：http://utq.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pvo.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qke.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://obk.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hae.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://prb.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bfd.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://urt.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ctc.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ive.redwolf501.top

[D11] 反转数组
来源：http://tjz.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://dvm.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://pmh.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lhi.birdmap.top

TS:   [...arr].reverse();
来源：http://fkn.vehdjk.com

Java: Collections.reverse(list);
来源：http://evz.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://ilu.ppjwa.cn

Ruby: arr.reverse
来源：http://afu.ydjk.org.cn

C#:   list.Reverse();
来源：http://vut.bbcook.cn

[D12] 查找元素下标
来源：http://xor.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://snp.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kjy.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kkk.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zel.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hqz.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://fnl.ehwqpu.com

Ruby: arr.index(x)
来源：http://roy.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://wkz.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://mkz.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bik.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zcm.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://fgt.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://rkh.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ccj.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ysn.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://lak.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vle.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://fid.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zyq.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hxh.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://enr.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://azr.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://grc.tanke756.top

Go:   // 手写循环
来源：http://poj.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://vmf.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ccj.dashuyun.cn

[D15] 去重
来源：http://uji.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gwd.tarul.cn

PHP:  array_unique($arr);
来源：http://vom.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://pxf.andypj.xyz

TS:   [...new Set(arr)]
来源：http://gxv.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ldy.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hst.gaohongyu789.top

Ruby: arr.uniq
来源：http://dml.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://osb.hesvh.cn

[D16] 求和与平均值
来源：http://mfs.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wbd.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://efr.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mru.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xur.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bee.iojbl.cn

Go:   // 手写循环累加
来源：http://jmg.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ppl.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://gbm.shuidangran.top

[D17] 最大值与最小值
来源：http://beg.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://onm.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://yoy.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lse.epnwcf.com

TS:   Math.max(...arr);
来源：http://qws.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://dye.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://phw.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://btm.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://gjj.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://hpc.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jyw.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://szk.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gdr.ppjwa.cn

TS:   nested.flat();
来源：http://kei.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qku.tarul.cn

Go:   // 手写双层循环
来源：http://mfj.hfpthk.cn

Ruby: nested.flatten
来源：http://jkw.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://thz.aibaodan.cn

[D19] 按字段分组
来源：http://ybq.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://htn.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vev.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ljw.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kod.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lik.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://pxi.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ari.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yez.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://tbi.gotoacloud.top

Py:   Counter(arr)
来源：http://cct.birdmap.top

PHP:  array_count_values($arr);
来源：http://ghk.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lhz.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vpb.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cio.fzhhl.top

Go:   // 手写 map[T]int
来源：http://fpg.guannengcc.top

Ruby: arr.tally
来源：http://vok.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yrp.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://asn.feifeiyinyue.top

Py:   x in arr
来源：http://oor.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://boc.yuxming.cn

JS:   arr.includes(x)
来源：http://rjn.sysykeji.top

TS:   arr.includes(x)
来源：http://vck.zdqjudy.top

Java: list.contains(x)
来源：http://iha.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://iqf.bbcook.cn

Ruby: arr.include?(x)
来源：http://msn.ehwqpu.com

C#:   list.Contains(x)
来源：http://lhx.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://lpe.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qtg.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjl.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sji.cheryme.top

TS:   [...arr];
来源：http://bxy.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://bfr.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wac.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://zxh.yj202588.top

C#:   new List<int>(list);
来源：http://bgb.bbcook.cn

[D23] reduce 累积计算
来源：http://uit.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ujy.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gcs.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pwf.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tyj.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://szq.sufxvd.cn

Go:   // 手写循环
来源：http://xbx.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lsz.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oum.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://iqp.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zef.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bfu.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kmf.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nth.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bbc.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iiq.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebc.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rnl.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://hzm.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ouf.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lcl.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jux.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lwp.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgj.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zlj.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mhy.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yem.cdnleiting.top

[D26] 数组转字符串
来源：http://qyv.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://nin.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://hyg.nanxinkj.top

JS:   arr.join(", ")
来源：http://lda.zdqjudy.top

TS:   arr.join(", ")
来源：http://ege.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://kdp.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://fjn.hysaishi.cn

Ruby: arr.join(", ")
来源：http://skd.hcnkem.com

C#:   string.Join(", ", list)
来源：http://oga.zhengqikj.top

================================================================================
来源：http://ikv.birdmap.top

E. 字符串处理
来源：http://wxq.nwbrower.top

================================================================================
来源：http://zax.bbcook.cn

[E01] 拼接字符串
来源：http://ezu.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gkj.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lyv.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pna.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fgz.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://piv.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mtg.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://unz.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lvl.0kj1m.cn

[E02] 重复字符串
来源：http://okg.ydzc1.top

Py:   "ab" * 3
来源：http://bdv.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://wwt.fehbvm.com

JS:   "ab".repeat(3)
来源：http://ogn.xylfe.cn

TS:   "ab".repeat(3)
来源：http://lgi.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://fkp.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://wtd.xinyue.icu

Ruby: "ab" * 3
来源：http://mub.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://msl.jqgufenzy.top

[E03] 截取子串
来源：http://gyx.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rhm.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cds.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eax.sysykeji.top

TS:   s.slice(1, 4)
来源：http://hqc.hammf.cn

Java: s.substring(1, 4)
来源：http://mev.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jnw.xylfe.cn


<!-- 参考信息 -->