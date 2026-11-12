代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bwa.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pda.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ovl.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gud.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://zvf.cucudq.cn

Go:   func add(a, b int) int
来源：http://ymc.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://keh.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://zml.9152youxi.cn

[C14] 泛型函数
来源：http://inb.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wmr.xuanzx.com

PHP:  // 无泛型
来源：http://igq.pycfn.com

JS:   // 无泛型
来源：http://fhj.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vdt.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ceq.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://biz.gogol.net.cn

Ruby: # 无泛型
来源：http://sfd.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sry.hcnkem.com

[C15] 解构 / 展开参数
来源：http://ueb.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xce.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://wkj.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azh.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zjk.9152youxi.cn

Java: // 无解构
来源：http://psn.nanxuanxn.top

Go:   // 无解构
来源：http://qto.ydzc1.top

Ruby: a, b = pair
来源：http://trn.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://apc.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ewm.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xsd.wangdashe.top

PHP:  // 无重载
来源：http://wbn.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zxp.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://eeg.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ehe.sweek.top

Go:   // 无重载：用不同函数名
来源：http://msf.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://hzc.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ohp.bbcook.cn

================================================================================
来源：http://rcp.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://oei.sufxvd.cn

================================================================================
来源：http://ybt.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://lgg.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kob.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://emb.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sjq.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wlw.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aff.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://jvo.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://fvy.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://onb.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://meq.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zxw.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvt.gogol.net.cn

JS:   arr.push(4);
来源：http://tms.zhongyouzk.top

TS:   arr.push(4);
来源：http://ise.jiagoushi.top

Java: list.add(4);
来源：http://dsu.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://bmo.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://byl.sjlbkw.cn

C#:   list.Add(4);
来源：http://axi.tanke756.top

[D03] 在指定位置插入元素
来源：http://qot.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://fns.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://srj.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tte.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://aww.zhixingplan.top

Java: list.add(0, 0);
来源：http://kaw.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pow.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zyk.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://utp.ppjwa.cn

[D04] 删除元素
来源：http://ukr.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rkj.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dma.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mua.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://guk.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nub.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://anx.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xmo.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wod.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://ziw.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dto.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jfq.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eiz.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://djg.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://kfh.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pct.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://whl.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uwa.tian-w.cn

[D06] 数组长度
来源：http://hhj.sjlbkw.cn

Py:   len(arr)
来源：http://ovf.shuidangran.top

PHP:  count($arr);
来源：http://ami.hcnkem.com

JS:   arr.length
来源：http://nvt.xuetiantiany.cn

TS:   arr.length
来源：http://lmf.gogol.net.cn

Java: list.size();
来源：http://ret.hcnkem.com

Go:   len(arr)
来源：http://btb.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://yuo.nwbrower.top

C#:   list.Count;
来源：http://jap.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://odz.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zmz.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qzz.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://uye.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://brs.hcnkem.com

Java: list.subList(1, 4);
来源：http://byk.sxryk.cn

Go:   arr[1:4]
来源：http://olu.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://fxg.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://ogv.vehdjk.com

[D08] 合并两个数组
来源：http://iqc.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://unj.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://yth.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ded.dashuyun.cn

TS:   [...a, ...b];
来源：http://bmt.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xxr.yvedp.cn

Go:   append(a, b...)
来源：http://svp.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://mjq.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://yhj.ehwqpu.com

[D09] 排序（升序）
来源：http://uri.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://dja.hfpthk.cn

PHP:  sort($arr);
来源：http://fvc.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://etc.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hwo.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sng.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pww.bbcook.cn

Ruby: arr.sort
来源：http://udp.uphjek.com

C#:   list.Sort();
来源：http://qnj.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bmf.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dfy.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cyq.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://duq.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ity.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vcs.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ynb.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ysf.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://knk.yfazqb.com

[D11] 反转数组
来源：http://icj.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://swy.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://zlf.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mjz.cdnleiting.top

TS:   [...arr].reverse();
来源：http://dij.ppjwa.cn

Java: Collections.reverse(list);
来源：http://mxg.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://nns.pengpengdd.cyou

Ruby: arr.reverse
来源：http://hpg.hnxiangtu.top

C#:   list.Reverse();
来源：http://wkv.cdnleiting.top

[D12] 查找元素下标
来源：http://bug.sweek.top

Py:   arr.index(x);  x in arr
来源：http://acc.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tqs.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ygs.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okb.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kua.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://eep.aibaodan.cn

Ruby: arr.index(x)
来源：http://nir.meibo888.top

C#:   list.IndexOf(x);
来源：http://msq.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://ric.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://shx.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhp.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://mwn.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://qxz.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nax.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dxd.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mda.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://veo.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://jwj.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vve.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gwf.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://oar.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://wdl.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://asn.chenjidiqi.icu

Go:   // 手写循环
来源：http://xdm.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xas.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nsl.gzhubu.top

[D15] 去重
来源：http://ksu.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uqt.yueranfly.top

PHP:  array_unique($arr);
来源：http://xzd.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://ajv.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://swd.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fpe.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://yos.wangshuangyany.cn

Ruby: arr.uniq
来源：http://uex.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://eph.uphjek.com

[D16] 求和与平均值
来源：http://ciq.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hnz.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dtu.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uwq.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jcy.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hhf.pycfn.com

Go:   // 手写循环累加
来源：http://oyh.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jee.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://egb.jinqigfzy.top

[D17] 最大值与最小值
来源：http://tpm.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://zqj.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://bdu.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fhq.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://rrc.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://lqr.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jsg.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://mbj.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://ohc.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://nvw.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kyv.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://fvf.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nnm.chenzaomai.com

TS:   nested.flat();
来源：http://vys.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ukc.jinqigufen.top

Go:   // 手写双层循环
来源：http://rwc.316326.xyz

Ruby: nested.flatten
来源：http://svx.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://myu.yueranfly.top

[D19] 按字段分组
来源：http://ecx.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://diu.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vtk.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fvl.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lwt.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gtb.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://uxq.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://icc.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sso.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://fsc.cqqwz.cn

Py:   Counter(arr)
来源：http://wmq.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://mrx.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wdk.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zhl.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yrm.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://zrs.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://glv.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zgq.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://ukv.gotoacloud.top

Py:   x in arr
来源：http://try.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://bxb.yuanzhike.top

JS:   arr.includes(x)
来源：http://tqe.ivvv.top

TS:   arr.includes(x)
来源：http://jfs.ybcxt.top

Java: list.contains(x)
来源：http://paw.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://dur.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://mvx.gotoacloud.top

C#:   list.Contains(x)
来源：http://wpd.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://izb.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fgi.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://llf.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rls.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://gmv.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://vje.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://ocp.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://urf.hesvh.cn

C#:   new List<int>(list);
来源：http://wfw.yj20258.top

[D23] reduce 累积计算
来源：http://ixg.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hog.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qms.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bsi.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bzw.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dnp.tianlin.xyz

Go:   // 手写循环
来源：http://gxu.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://itb.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yfc.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://muz.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tqm.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ixg.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vsp.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mmq.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cne.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rhm.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qhi.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://spx.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://yqf.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ysl.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aul.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fpw.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qoy.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fsr.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cfy.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://teo.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://otm.jianghu66.top

[D26] 数组转字符串
来源：http://wox.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://uhk.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://aot.gzhubu.top

JS:   arr.join(", ")
来源：http://wpq.ivvv.top

TS:   arr.join(", ")
来源：http://vzv.dianchejie.cn

Java: String.join(", ", list)
来源：http://bte.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://qrq.cdnleiting.top

Ruby: arr.join(", ")
来源：http://qpa.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://idv.yuanzhike.top

================================================================================
来源：http://sza.yangfankeji.com

E. 字符串处理
来源：http://ukh.hcnkem.com

================================================================================
来源：http://lef.fktsv.cn

[E01] 拼接字符串
来源：http://vjj.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwc.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uxd.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mva.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ozh.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfu.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oty.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oes.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jqs.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://svj.zhiwuduotai.top

Py:   "ab" * 3
来源：http://jra.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://gnc.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://qed.zycfv.cn

TS:   "ab".repeat(3)
来源：http://qdt.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://xid.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://waq.epnwcf.com

Ruby: "ab" * 3
来源：http://bxj.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://odt.xziqi.cn

[E03] 截取子串
来源：http://iuh.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zhw.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kea.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ylt.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://yti.hfpthk.cn

Java: s.substring(1, 4)
来源：http://gtg.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vmj.shanyushiyangkeji.top


<!-- 参考信息 -->