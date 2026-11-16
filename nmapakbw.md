代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://igb.hfpthk.cn

Go:   func add(a, b int) int
来源：http://lqz.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oon.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://gmi.jianghu66.top

[C14] 泛型函数
来源：http://hgf.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ozj.nwbrower.top

PHP:  // 无泛型
来源：http://fhl.fzhhl.top

JS:   // 无泛型
来源：http://edn.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tcb.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uyh.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vmz.chenzaomai.com

Ruby: # 无泛型
来源：http://rzh.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xcq.xziqi.cn

[C15] 解构 / 展开参数
来源：http://rsy.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nlc.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://gdj.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cvm.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zwa.xuetiantiany.cn

Java: // 无解构
来源：http://qbs.snrcjt.cn

Go:   // 无解构
来源：http://zqq.cheryme.top

Ruby: a, b = pair
来源：http://lea.yueranfly.top

C#:   var (a, b) = pair;
来源：http://jzr.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://vfs.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pqz.tarul.cn

PHP:  // 无重载
来源：http://qpi.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://fkh.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://atf.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tyo.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://tgq.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://ibc.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://czx.shanyushiyangkeji.top

================================================================================
来源：http://cqb.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://lfc.guannengcc.top

================================================================================
来源：http://zpy.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://ffx.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vyr.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uxj.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gza.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ocl.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nnm.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://oxp.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://kdi.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://voe.jiagoushi.top

[D02] 追加元素到末尾
来源：http://llg.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://evh.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jtk.tianlin.xyz

JS:   arr.push(4);
来源：http://mjn.hywenlv.cn

TS:   arr.push(4);
来源：http://qpm.yonumen.top

Java: list.add(4);
来源：http://pde.yongpay.top

Go:   arr = append(arr, 4)
来源：http://thr.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://kys.fzhhl.top

C#:   list.Add(4);
来源：http://ugi.bbcook.cn

[D03] 在指定位置插入元素
来源：http://pup.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://kvp.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://frm.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bpd.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://jmj.vqdsnc.cn

Java: list.add(0, 0);
来源：http://oer.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://siv.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cmc.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://jca.xziqi.cn

[D04] 删除元素
来源：http://bos.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xom.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twq.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tsi.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://dej.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iyo.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hxo.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ewq.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://teo.ydjk.org.cn

[D05] 访问与修改元素
来源：http://res.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rkw.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sdc.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jmf.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://fba.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://fse.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://eyn.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nhg.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kia.birdmap.top

[D06] 数组长度
来源：http://lqn.iojbl.cn

Py:   len(arr)
来源：http://djs.cashguo.top

PHP:  count($arr);
来源：http://iid.ehwqpu.com

JS:   arr.length
来源：http://vou.zhijiandao.cn

TS:   arr.length
来源：http://unj.shangyingyoupin.top

Java: list.size();
来源：http://scb.yj20258.top

Go:   len(arr)
来源：http://gsx.yueranfly.top

Ruby: arr.length; arr.size
来源：http://irx.uphjek.com

C#:   list.Count;
来源：http://ohh.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://suc.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jxg.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://csv.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://pna.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://xja.mhx1999.top

Java: list.subList(1, 4);
来源：http://nzv.fktsv.cn

Go:   arr[1:4]
来源：http://djo.gotoacloud.top

Ruby: arr[1, 3]
来源：http://gxh.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://yqv.ehwqpu.com

[D08] 合并两个数组
来源：http://yax.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://njh.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://eok.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eus.yanxiufei.cn

TS:   [...a, ...b];
来源：http://dzo.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrs.9152youxi.cn

Go:   append(a, b...)
来源：http://yez.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://jfx.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://iim.pengpengdd.cyou

[D09] 排序（升序）
来源：http://bye.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://yrx.vqdsnc.cn

PHP:  sort($arr);
来源：http://ejt.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vyf.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uar.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://amq.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mbo.uphjek.com

Ruby: arr.sort
来源：http://boh.316326.xyz

C#:   list.Sort();
来源：http://vih.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vdk.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dfz.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ylu.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bnw.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sdd.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dpm.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nuy.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tof.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gjv.zdbjq.cn

[D11] 反转数组
来源：http://omf.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://ufl.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://vfm.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xoc.xylfe.cn

TS:   [...arr].reverse();
来源：http://vqe.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://liu.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://eyo.ivvv.top

Ruby: arr.reverse
来源：http://geq.nanxuanxn.top

C#:   list.Reverse();
来源：http://bpk.gogol.net.cn

[D12] 查找元素下标
来源：http://qwo.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://acv.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nmn.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nae.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pvz.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sky.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://bad.birdmap.top

Ruby: arr.index(x)
来源：http://muz.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://gey.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://vbl.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sxe.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bii.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://ijs.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://fqe.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://buf.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ggi.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dsq.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://reg.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://lfd.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ncw.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vgz.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://qiw.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://ucj.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vpb.cqqwz.cn

Go:   // 手写循环
来源：http://oas.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wkj.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fmr.dashuyun.cn

[D15] 去重
来源：http://jlv.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qua.chenlongwang.top

PHP:  array_unique($arr);
来源：http://gze.cucudq.cn

JS:   [...new Set(arr)]
来源：http://itr.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://vme.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://szc.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://jlx.zhijiandao.cn

Ruby: arr.uniq
来源：http://jmj.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://mqm.jqgfzy.top

[D16] 求和与平均值
来源：http://iip.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cve.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fpv.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uiq.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofx.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogz.yj202588.top

Go:   // 手写循环累加
来源：http://srp.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gle.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://hhl.bbcook.cn

[D17] 最大值与最小值
来源：http://ycy.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://lyi.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://ndz.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ajx.fktsv.cn

TS:   Math.max(...arr);
来源：http://mno.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hyv.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qvg.316326.xyz

Ruby: arr.max;  arr.min
来源：http://iuv.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://whv.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://xjp.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uxx.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://hmn.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://elr.zhiwuduotai.top

TS:   nested.flat();
来源：http://dei.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://raj.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://sjh.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://chz.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fdd.9152youxi.cn

[D19] 按字段分组
来源：http://sxc.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pmw.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vgs.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fys.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iyd.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://swv.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://rcz.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zwe.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dcg.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://sdl.yfazqb.com

Py:   Counter(arr)
来源：http://zmq.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://klq.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hjh.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mjh.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kpo.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://qrm.yj202588.top

Ruby: arr.tally
来源：http://lec.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wpx.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://nzn.zhongyouzk.top

Py:   x in arr
来源：http://wyy.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://psb.kuanghao11.cn

JS:   arr.includes(x)
来源：http://bqu.vqdsnc.cn

TS:   arr.includes(x)
来源：http://hzk.nwbrower.top

Java: list.contains(x)
来源：http://yre.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://zyo.yvedp.cn

Ruby: arr.include?(x)
来源：http://mrl.redwolf501.top

C#:   list.Contains(x)
来源：http://kwj.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://xzm.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yhe.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vad.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eon.cheryme.top

TS:   [...arr];
来源：http://tqi.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://ldx.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://vlj.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://wqi.9152youxi.cn

C#:   new List<int>(list);
来源：http://vzi.vqdsnc.cn

[D23] reduce 累积计算
来源：http://jdp.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lpl.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dcr.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eny.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rpk.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mbw.sufxvd.cn

Go:   // 手写循环
来源：http://qrb.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jax.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pqa.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://abo.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xjw.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://noi.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gkm.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://faw.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dij.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jly.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oab.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lds.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://qbm.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sov.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ule.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yhv.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uar.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lyl.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pam.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jdg.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://onw.jinqigfzy.top

[D26] 数组转字符串
来源：http://zkd.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://ioq.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://rpk.ivvv.top

JS:   arr.join(", ")
来源：http://qgk.andypj.xyz

TS:   arr.join(", ")
来源：http://njy.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://ywh.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://rmo.yongpay.top

Ruby: arr.join(", ")
来源：http://pll.52xcode.cn

C#:   string.Join(", ", list)
来源：http://ghp.xziqi.cn

================================================================================
来源：http://lnp.zhixingplan.top

E. 字符串处理
来源：http://amf.fehbvm.com

================================================================================
来源：http://edh.uphjek.com

[E01] 拼接字符串
来源：http://alr.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tgr.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://utx.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://skn.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxn.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gzd.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://guk.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cwl.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wpv.xuanzx.com

[E02] 重复字符串
来源：http://tyl.jinqigufen.top

Py:   "ab" * 3
来源：http://crn.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://ity.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://hfd.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://xux.daxiang520.top

Java: "ab".repeat(3)
来源：http://bkd.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://fzx.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://mcz.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dkj.yj20258888.top

[E03] 截取子串
来源：http://dxn.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oba.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lej.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.316326.xyz

TS:   s.slice(1, 4)
来源：http://vpp.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://erv.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wer.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://rlw.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://bce.cucudq.cn

[E04] 查找子串位置
来源：http://rez.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://fls.ppjwa.cn


<!-- 参考信息 -->