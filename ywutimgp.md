代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://iqm.xziqi.cn

Go:   func add(a, b int) int
来源：http://rwo.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://djj.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://qem.havefunace.top

[C14] 泛型函数
来源：http://fde.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oxq.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://wza.hnqzz.top

JS:   // 无泛型
来源：http://aei.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ape.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://chu.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gry.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://mbs.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oqq.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://bhd.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ebf.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://xrw.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ojf.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://byd.hysaishi.cn

Java: // 无解构
来源：http://sop.hfpthk.cn

Go:   // 无解构
来源：http://rsn.uphjek.com

Ruby: a, b = pair
来源：http://dkr.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://oyn.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://jxe.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qgz.ydzc1.top

PHP:  // 无重载
来源：http://cpg.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://bde.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://aec.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xxa.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://flx.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://lsr.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jwo.bjfxy.top

================================================================================
来源：http://utp.tanke756.top

D. 数组 / 列表 / 集合
来源：http://snh.hnxiangtu.top

================================================================================
来源：http://lnj.yongpay.top

[D01] 创建数组 / 列表
来源：http://uec.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eec.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aux.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kbl.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://sbh.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yiy.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://pgc.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://mwo.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://klo.jianghu66.top

[D02] 追加元素到末尾
来源：http://vus.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rkd.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vpc.jianghu66.top

JS:   arr.push(4);
来源：http://utr.yongpay.top

TS:   arr.push(4);
来源：http://ciz.tarul.cn

Java: list.add(4);
来源：http://cil.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://khg.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://gwy.vehdjk.com

C#:   list.Add(4);
来源：http://hgo.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://rlj.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://pna.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lre.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qlf.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://mys.iojbl.cn

Java: list.add(0, 0);
来源：http://swx.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://fnm.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://czv.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://ndd.ywan-chungtsiang.top

[D04] 删除元素
来源：http://knk.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://goi.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgw.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jkl.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://zkv.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kcv.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shi.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://geh.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tux.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://qrs.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gce.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rli.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dqc.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://hxh.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://hza.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://orm.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yxf.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ehh.hammf.cn

[D06] 数组长度
来源：http://yus.hongshengwenyu.top

Py:   len(arr)
来源：http://aka.0kj1m.cn

PHP:  count($arr);
来源：http://vpp.wangshuangyany.cn

JS:   arr.length
来源：http://mse.jinyuanbaomall.cn

TS:   arr.length
来源：http://ihx.yuanzhike.top

Java: list.size();
来源：http://kyl.daria6918.cn

Go:   len(arr)
来源：http://zax.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://qaq.fehbvm.com

C#:   list.Count;
来源：http://uts.andypj.xyz

[D07] 切片 / 取子数组
来源：http://tdy.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://saq.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://wre.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://nkb.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://wcr.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://yyt.jinqigfzy.top

Go:   arr[1:4]
来源：http://ifg.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://fip.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://ebh.ehwqpu.com

[D08] 合并两个数组
来源：http://lzf.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://nbw.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://fxd.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nhs.zhongyouzk.top

TS:   [...a, ...b];
来源：http://eba.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iba.gotoacloud.top

Go:   append(a, b...)
来源：http://vvq.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://ezz.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://thu.gogol.net.cn

[D09] 排序（升序）
来源：http://yzn.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://wmx.redwolf501.top

PHP:  sort($arr);
来源：http://pkh.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wvt.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pzs.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bre.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nry.zdbjq.cn

Ruby: arr.sort
来源：http://esp.jqgfzy.top

C#:   list.Sort();
来源：http://zyg.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qcz.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kae.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xlk.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pty.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jko.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xyg.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rpl.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xos.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uih.tianlin.xyz

[D11] 反转数组
来源：http://wgf.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ung.sweek.top

PHP:  array_reverse($arr);
来源：http://qkj.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ksf.dianchejie.cn

TS:   [...arr].reverse();
来源：http://lhl.jyoumei.cn

Java: Collections.reverse(list);
来源：http://wbf.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://say.hesvh.cn

Ruby: arr.reverse
来源：http://qcq.yanxiufei.cn

C#:   list.Reverse();
来源：http://kez.guannengcc.top

[D12] 查找元素下标
来源：http://yon.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://zvi.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlg.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dzt.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xxn.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ybe.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://zvs.yuanzhike.top

Ruby: arr.index(x)
来源：http://dxk.yueranfly.top

C#:   list.IndexOf(x);
来源：http://hnk.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://elx.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwl.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ipx.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://rmk.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://tby.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hhs.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kzh.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://eja.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rqu.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://tvn.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rff.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gjw.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://lto.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://zav.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://cka.daxiang520.top

Go:   // 手写循环
来源：http://ytg.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://mzt.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yps.sweek.top

[D15] 去重
来源：http://vqq.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gyn.yj20258888.top

PHP:  array_unique($arr);
来源：http://cuh.hesvh.cn

JS:   [...new Set(arr)]
来源：http://vqp.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://kyj.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mne.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://mgv.dashuyun.cn

Ruby: arr.uniq
来源：http://rxe.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://pjq.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://kiu.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bot.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ajb.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://enk.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wld.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://egf.cqqwz.cn

Go:   // 手写循环累加
来源：http://uzi.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ytg.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://nyg.zhoulong.xyz

[D17] 最大值与最小值
来源：http://htx.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://eum.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://lgv.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pzu.jiagoushi.top

TS:   Math.max(...arr);
来源：http://zkb.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hyo.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kjb.yj20258.top

Ruby: arr.max;  arr.min
来源：http://asn.yj20258.top

C#:   list.Max();  list.Min()
来源：http://xsf.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://gve.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qsf.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://ahv.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pml.uphjek.com

TS:   nested.flat();
来源：http://sxv.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bke.nanxuanxn.top

Go:   // 手写双层循环
来源：http://wly.fehbvm.com

Ruby: nested.flatten
来源：http://ith.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zqe.fktsv.cn

[D19] 按字段分组
来源：http://cqm.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://euf.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sqj.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eiu.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pph.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://byj.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://hmv.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lrk.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cek.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://jvy.gzhubu.top

Py:   Counter(arr)
来源：http://diw.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://xsy.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yre.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mrz.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yjz.yj20258.top

Go:   // 手写 map[T]int
来源：http://rvl.fktsv.cn

Ruby: arr.tally
来源：http://vnc.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwd.yj202588.top

[D21] 判断是否包含某元素
来源：http://llv.xuanzx.com

Py:   x in arr
来源：http://lhp.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://jxb.havefunace.top

JS:   arr.includes(x)
来源：http://lvi.bjfxy.top

TS:   arr.includes(x)
来源：http://cvz.xziqi.cn

Java: list.contains(x)
来源：http://jil.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://urs.andypj.xyz

Ruby: arr.include?(x)
来源：http://cde.fengsongda.top

C#:   list.Contains(x)
来源：http://iqq.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://dke.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhw.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xyz.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lln.ehwqpu.com

TS:   [...arr];
来源：http://rag.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://rqm.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://zqd.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://ztn.ppjwa.cn

C#:   new List<int>(list);
来源：http://kui.dashuyun.cn

[D23] reduce 累积计算
来源：http://hrd.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xop.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fon.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ayu.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skm.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hgl.hongshengwenyu.top

Go:   // 手写循环
来源：http://foj.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://axs.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vfn.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://keh.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ymk.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mxl.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ink.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cry.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://khx.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ciz.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gev.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucf.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://zsm.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://avd.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xse.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tsv.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://drf.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hlt.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pgj.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qiv.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://slm.epnwcf.com

[D26] 数组转字符串
来源：http://ubd.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://jyq.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://nyo.hnxiangtu.top

JS:   arr.join(", ")
来源：http://ait.yvedp.cn

TS:   arr.join(", ")
来源：http://esz.guowangkeji.top

Java: String.join(", ", list)
来源：http://vtx.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://jws.9152youxi.cn

Ruby: arr.join(", ")
来源：http://mww.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://mjj.316326.xyz

================================================================================
来源：http://pyq.9152youxi.cn

E. 字符串处理
来源：http://ore.shanyushiyangkeji.top

================================================================================
来源：http://dbi.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://jwe.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mrg.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kih.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bhm.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpb.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://krd.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mys.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rbv.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lpw.0kj1m.cn

[E02] 重复字符串
来源：http://jaq.gotoacloud.top

Py:   "ab" * 3
来源：http://etp.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://vkl.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://sta.redwolf501.top

TS:   "ab".repeat(3)
来源：http://mna.chenzaomai.com

Java: "ab".repeat(3)
来源：http://tnu.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://yqc.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://mgr.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vhj.hammf.cn

[E03] 截取子串
来源：http://nqz.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hfl.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iof.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eej.fengsongda.top

TS:   s.slice(1, 4)
来源：http://yru.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://ych.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vwo.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mul.ivvv.top

C#:   s.Substring(1, 3)
来源：http://vbe.shuidangran.top

[E04] 查找子串位置
来源：http://yqn.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://ejm.0kj1m.cn


<!-- 参考信息 -->