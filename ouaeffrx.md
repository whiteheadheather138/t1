代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://rfm.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://ywz.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://ihw.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uqg.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://ecp.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://khb.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gwi.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://wyj.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://irt.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ryc.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uvp.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqe.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dqh.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://ozc.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sqn.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://hmf.9152youxi.cn

[C14] 泛型函数
来源：http://adg.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rdz.redwolf501.top

PHP:  // 无泛型
来源：http://com.havefunace.top

JS:   // 无泛型
来源：http://hbr.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gqg.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tab.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fus.svipenyu.cn

Ruby: # 无泛型
来源：http://ptc.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qsb.hcnkem.com

[C15] 解构 / 展开参数
来源：http://xij.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sbc.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://rqi.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ujf.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hve.xylfe.cn

Java: // 无解构
来源：http://ttn.dianchejie.cn

Go:   // 无解构
来源：http://gnk.yuxming.cn

Ruby: a, b = pair
来源：http://ooy.tian-w.cn

C#:   var (a, b) = pair;
来源：http://rnv.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://txl.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hlw.jianghu66.top

PHP:  // 无重载
来源：http://reo.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ron.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://qru.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://npi.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://fid.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://efx.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlm.zdbjq.cn

================================================================================
来源：http://gtw.pycfn.com

D. 数组 / 列表 / 集合
来源：http://ndf.wangdashe.top

================================================================================
来源：http://rdi.ivvv.top

[D01] 创建数组 / 列表
来源：http://zwl.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wch.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vfh.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bzt.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://exo.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cfu.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://zpj.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://amb.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://alj.nwbrower.top

[D02] 追加元素到末尾
来源：http://bcs.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xtr.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oup.yj20258888.top

JS:   arr.push(4);
来源：http://rvz.hysaishi.cn

TS:   arr.push(4);
来源：http://ygc.cucudq.cn

Java: list.add(4);
来源：http://ebg.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://bbh.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://coq.daxiang520.top

C#:   list.Add(4);
来源：http://iwf.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://tsm.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://pkj.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kfe.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://umv.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://wbh.cashguo.top

Java: list.add(0, 0);
来源：http://ood.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://onv.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ycr.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://jpc.chenzaomai.com

[D04] 删除元素
来源：http://hlo.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fhz.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kic.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fxi.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://tcp.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jji.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zig.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qww.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eza.hysaishi.cn

[D05] 访问与修改元素
来源：http://gab.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wuo.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rlw.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ksy.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://veh.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://icm.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://edy.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jbi.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://col.mhx1999.top

[D06] 数组长度
来源：http://sfs.shanyushiyangkeji.top

Py:   len(arr)
来源：http://pxc.hcnkem.com

PHP:  count($arr);
来源：http://oly.jyoumei.cn

JS:   arr.length
来源：http://rap.ivvv.top

TS:   arr.length
来源：http://shh.jyoumei.cn

Java: list.size();
来源：http://ktx.mhx1999.top

Go:   len(arr)
来源：http://vuz.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://dik.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://qaa.daria6918.cn

[D07] 切片 / 取子数组
来源：http://pqx.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zcw.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://emb.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://xrx.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://vuc.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://daz.haohaochexian.top

Go:   arr[1:4]
来源：http://wvx.sysykeji.top

Ruby: arr[1, 3]
来源：http://tlk.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://wgx.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://izl.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://dpp.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://mph.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://uni.cashguo.top

TS:   [...a, ...b];
来源：http://jwn.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xgo.yonumen.top

Go:   append(a, b...)
来源：http://voc.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://cru.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://uzq.bbcook.cn

[D09] 排序（升序）
来源：http://aet.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://qfa.cucudq.cn

PHP:  sort($arr);
来源：http://ucd.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cas.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fyn.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rom.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vkm.zhongyouzk.top

Ruby: arr.sort
来源：http://gyb.hesvh.cn

C#:   list.Sort();
来源：http://jqi.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://awa.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ckx.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bfu.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvo.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmj.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://udl.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lln.hcnkem.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dgt.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://siq.pycfn.com

[D11] 反转数组
来源：http://vab.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://oub.316326.xyz

PHP:  array_reverse($arr);
来源：http://hup.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rtx.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://pwc.yangfankeji.com

Java: Collections.reverse(list);
来源：http://cio.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://pii.yj20258.top

Ruby: arr.reverse
来源：http://mer.chenzaomai.com

C#:   list.Reverse();
来源：http://elj.chenzaomai.com

[D12] 查找元素下标
来源：http://cfr.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://stt.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eto.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nwv.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxp.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://job.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://yqd.hesvh.cn

Ruby: arr.index(x)
来源：http://wde.xylfe.cn

C#:   list.IndexOf(x);
来源：http://rlt.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://ozp.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zaf.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yjg.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://mng.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://jys.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fzi.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dmb.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kdi.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lcw.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://pgn.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://prz.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kcc.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://tuw.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://laj.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ldg.ppjwa.cn

Go:   // 手写循环
来源：http://shh.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nkz.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uey.jlsjyb.cn

[D15] 去重
来源：http://ddx.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vyp.yuanzhike.top

PHP:  array_unique($arr);
来源：http://pts.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://bnf.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://zfk.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ryn.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dns.yfazqb.com

Ruby: arr.uniq
来源：http://ani.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://bht.quarkkingdee.top

[D16] 求和与平均值
来源：http://ldk.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pip.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://udz.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ido.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxv.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://agj.xinyue.icu

Go:   // 手写循环累加
来源：http://kzv.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://daz.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://yjy.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://xnf.uphjek.com

Py:   max(arr);  min(arr)
来源：http://fqv.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://rdp.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lvn.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://myx.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fce.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsy.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://prm.hammf.cn

C#:   list.Max();  list.Min()
来源：http://pwj.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://uay.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bul.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://sjd.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xmw.jlsjyb.cn

TS:   nested.flat();
来源：http://efe.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cef.epnwcf.com

Go:   // 手写双层循环
来源：http://nos.uphjek.com

Ruby: nested.flatten
来源：http://vmg.jinqigufen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ddu.shanyushiyangtech.top

[D19] 按字段分组
来源：http://qws.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wxp.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ise.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uza.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rfg.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ymf.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://sun.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gym.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zkq.yonumen.top

[D20] 统计每个元素出现次数
来源：http://axl.hcnkem.com

Py:   Counter(arr)
来源：http://tzb.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://hbs.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocy.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubf.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jpe.chenjidiqi.icu

Go:   // 手写 map[T]int
来源：http://kxi.yfazqb.com

Ruby: arr.tally
来源：http://reg.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iyk.nwbrower.top

[D21] 判断是否包含某元素
来源：http://klm.daxiang520.top

Py:   x in arr
来源：http://ygb.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://jns.cdnleiting.top

JS:   arr.includes(x)
来源：http://jhp.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://dgt.gotoacloud.top

Java: list.contains(x)
来源：http://pjy.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://pcw.bbcook.cn

Ruby: arr.include?(x)
来源：http://mbs.guannengcc.top

C#:   list.Contains(x)
来源：http://hsd.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://sji.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bov.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gxi.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xfc.xuetiantiany.cn

TS:   [...arr];
来源：http://fpt.xuanzx.com

Java: new ArrayList<>(list);
来源：http://ryj.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fmb.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://msx.ivvv.top

C#:   new List<int>(list);
来源：http://uel.jqgfzy.top

[D23] reduce 累积计算
来源：http://fuz.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gxn.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lha.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpq.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cob.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kse.wangdashe.top

Go:   // 手写循环
来源：http://vlo.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oen.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bse.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://flr.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tus.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bwa.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wco.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xdd.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cjw.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://okv.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://can.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fgk.tarul.cn

[D25] Set 集合去重与交并差
来源：http://qde.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ray.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ghg.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://doo.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ysc.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ubs.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kpl.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gth.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqg.guowangkeji.top

[D26] 数组转字符串
来源：http://pwg.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://art.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://imb.cqqwz.cn

JS:   arr.join(", ")
来源：http://ynl.c1oappe.top

TS:   arr.join(", ")
来源：http://wnx.birdmap.top

Java: String.join(", ", list)
来源：http://efw.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://bcg.52xcode.cn

Ruby: arr.join(", ")
来源：http://pvv.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://eki.jqgfzy.top

================================================================================
来源：http://akt.ctjpmb.com

E. 字符串处理
来源：http://bmr.aibaodan.cn

================================================================================
来源：http://qlh.zhengqikj.top

[E01] 拼接字符串
来源：http://nhb.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zms.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qrz.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyw.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uub.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mdz.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://szi.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aup.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ncn.zhongyouzk.top

[E02] 重复字符串
来源：http://wrp.chenlongwang.top

Py:   "ab" * 3
来源：http://ugh.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://wuh.fehbvm.com

JS:   "ab".repeat(3)
来源：http://jnb.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://vva.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://oyc.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://dtu.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://xkk.epnwcf.com


<!-- 参考信息 -->