代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://wyc.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://qqe.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zyw.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://zgf.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mel.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcs.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xph.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://trf.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bgt.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://xkw.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ena.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://cpr.yanxiufei.cn

[C14] 泛型函数
来源：http://lxj.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tki.jyoumei.cn

PHP:  // 无泛型
来源：http://aqq.sjlbkw.cn

JS:   // 无泛型
来源：http://bqq.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wvv.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tun.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xua.yongpay.top

Ruby: # 无泛型
来源：http://leh.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yir.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://uwh.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ijw.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://dkc.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://abq.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://agx.9152youxi.cn

Java: // 无解构
来源：http://ywv.yongpay.top

Go:   // 无解构
来源：http://quw.meibo888.top

Ruby: a, b = pair
来源：http://zev.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://lio.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://qqg.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ypt.ydjk.org.cn

PHP:  // 无重载
来源：http://ggx.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cxn.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://maf.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tae.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://rgs.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://gof.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kvh.ppjwa.cn

================================================================================
来源：http://ogz.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://fgq.hnxiangtu.top

================================================================================
来源：http://zkb.jianghu66.top

[D01] 创建数组 / 列表
来源：http://tgl.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ujm.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jvj.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mav.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zag.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mps.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://elh.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://son.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://juc.havefunace.top

[D02] 追加元素到末尾
来源：http://hjw.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ptx.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uym.yangfankeji.com

JS:   arr.push(4);
来源：http://aqz.ivvv.top

TS:   arr.push(4);
来源：http://uyb.zhixingplan.top

Java: list.add(4);
来源：http://its.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://lvb.ybcxt.top

Ruby: arr << 4; arr.push(5)
来源：http://uqg.ctjpmb.com

C#:   list.Add(4);
来源：http://bnq.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://emv.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://vfq.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zng.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uuv.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://xdr.jinqigfzy.top

Java: list.add(0, 0);
来源：http://qfo.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://tac.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://csr.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://nro.52xcode.cn

[D04] 删除元素
来源：http://onv.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ffy.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://krt.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nvo.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://urh.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sid.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tnw.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pjr.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oug.xinyue.icu

[D05] 访问与修改元素
来源：http://zgg.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fen.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vho.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hiz.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://rwa.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://txr.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://qcu.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oqj.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hya.yuanzhike.top

[D06] 数组长度
来源：http://bub.sufxvd.cn

Py:   len(arr)
来源：http://xdu.tanke756.top

PHP:  count($arr);
来源：http://txk.fzhhl.top

JS:   arr.length
来源：http://rfu.ctjpmb.com

TS:   arr.length
来源：http://luv.yanxiufei.cn

Java: list.size();
来源：http://dvk.ywan-chungtsiang.top

Go:   len(arr)
来源：http://grm.cashguo.top

Ruby: arr.length; arr.size
来源：http://oer.zhiwuduotai.top

C#:   list.Count;
来源：http://vlh.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://eyl.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qwk.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://eio.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://kxc.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://wze.hesvh.cn

Java: list.subList(1, 4);
来源：http://ghy.fengsongda.top

Go:   arr[1:4]
来源：http://zvp.guannengcc.top

Ruby: arr[1, 3]
来源：http://apt.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://nnf.guowangkeji.top

[D08] 合并两个数组
来源：http://wjl.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://ucd.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://occ.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://btb.jinqigfzy.top

TS:   [...a, ...b];
来源：http://jht.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jfq.aizwys.cn

Go:   append(a, b...)
来源：http://skk.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://icm.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://zfd.pengpengdd.cyou

[D09] 排序（升序）
来源：http://kue.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://vuc.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://xlv.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fqq.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://afi.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://eas.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oxc.yonumen.top

Ruby: arr.sort
来源：http://aip.yonumen.top

C#:   list.Sort();
来源：http://sgk.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjj.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kcx.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jjh.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbl.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wgn.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxr.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oor.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ioy.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jnz.gotoacloud.top

[D11] 反转数组
来源：http://yxh.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sqr.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://bcc.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bus.daria6918.cn

TS:   [...arr].reverse();
来源：http://mzm.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://rcq.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://qcb.cucudq.cn

Ruby: arr.reverse
来源：http://nyg.nanxinkj.top

C#:   list.Reverse();
来源：http://shm.zhiwuduotai.top

[D12] 查找元素下标
来源：http://lyt.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://wtv.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rim.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bmi.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jow.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sft.sweek.top

Go:   slices.Index(arr, x)
来源：http://eiu.sxryk.cn

Ruby: arr.index(x)
来源：http://izg.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://djt.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://zdd.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cob.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vjt.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://bqm.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://myb.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yer.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xgk.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://afl.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fkh.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://kwp.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mrl.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uys.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://vlm.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://vxh.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lmg.ydjk.org.cn

Go:   // 手写循环
来源：http://non.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://vgt.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cfb.ybcxt.top

[D15] 去重
来源：http://seq.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcp.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://lpl.ybcxt.top

JS:   [...new Set(arr)]
来源：http://prr.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://cwp.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sar.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://khr.yanxiufei.cn

Ruby: arr.uniq
来源：http://gjn.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://yiw.yfazqb.com

[D16] 求和与平均值
来源：http://mif.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayi.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zmj.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrs.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xxy.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mkj.ctjpmb.com

Go:   // 手写循环累加
来源：http://vox.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nug.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://zap.redwolf501.top

[D17] 最大值与最小值
来源：http://xho.hammf.cn

Py:   max(arr);  min(arr)
来源：http://amx.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://moh.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rtr.9152youxi.cn

TS:   Math.max(...arr);
来源：http://gtc.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://qlc.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://njz.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://xrg.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://qma.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://qmq.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lvw.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://cjy.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bud.hongshengwenyu.top

TS:   nested.flat();
来源：http://rwt.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://srd.vehdjk.com

Go:   // 手写双层循环
来源：http://uku.hammf.cn

Ruby: nested.flatten
来源：http://xpw.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xrh.zhiwuduotai.top

[D19] 按字段分组
来源：http://eup.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jvn.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ksi.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iso.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkn.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mxh.316326.xyz

Go:   // 手写 map[string][]T
来源：http://ags.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://bew.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nan.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://ztn.hywenlv.cn

Py:   Counter(arr)
来源：http://hoc.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://rpn.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whj.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://icm.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://miq.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://aay.0kj1m.cn

Ruby: arr.tally
来源：http://fds.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufr.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://oii.nanxuanxn.top

Py:   x in arr
来源：http://pdl.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://soc.yueranfly.top

JS:   arr.includes(x)
来源：http://blm.yanxiufei.cn

TS:   arr.includes(x)
来源：http://yjt.316326.xyz

Java: list.contains(x)
来源：http://jjz.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://oiq.vehdjk.com

Ruby: arr.include?(x)
来源：http://rbt.yuxming.cn

C#:   list.Contains(x)
来源：http://uzy.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://vlg.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tac.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yuz.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xzf.zhiwuduotai.top

TS:   [...arr];
来源：http://bvu.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://qsb.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://xpc.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://nwn.zhengqikj.top

C#:   new List<int>(list);
来源：http://uez.hnqzz.top

[D23] reduce 累积计算
来源：http://eok.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bvz.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tam.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://coa.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uzl.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tfq.smart0.xyz

Go:   // 手写循环
来源：http://gbf.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mxe.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hpa.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://ldp.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yal.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://edv.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://peh.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mcv.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xuu.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tpx.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qbo.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lwc.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://xma.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vdc.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rzg.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tvt.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ias.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://izl.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://odm.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mdc.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gwk.vqdsnc.cn

[D26] 数组转字符串
来源：http://vkv.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://toj.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://wmv.ydzc1.top

JS:   arr.join(", ")
来源：http://flz.ybcxt.top

TS:   arr.join(", ")
来源：http://qpd.yonumen.top

Java: String.join(", ", list)
来源：http://uua.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://mjm.316326.xyz

Ruby: arr.join(", ")
来源：http://yak.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://vfx.sxryk.cn

================================================================================
来源：http://qxq.jqgufenzy.top

E. 字符串处理
来源：http://knd.bjfxy.top

================================================================================
来源：http://bvt.jinqigufen.top

[E01] 拼接字符串
来源：http://enk.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bvc.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ozc.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cfn.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dkh.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wgs.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vjy.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wqo.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://isw.pengpengdd.cyou

[E02] 重复字符串
来源：http://cbx.epnwcf.com

Py:   "ab" * 3
来源：http://wbw.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://lid.uphjek.com

JS:   "ab".repeat(3)
来源：http://lzj.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://kgb.gogol.net.cn

Java: "ab".repeat(3)
来源：http://lpp.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://gqf.xziqi.cn

Ruby: "ab" * 3
来源：http://lez.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rff.yonumen.top

[E03] 截取子串
来源：http://nto.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hfx.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ecx.vehdjk.com


<!-- 参考信息 -->