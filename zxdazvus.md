代发 wailian999

[C14] 泛型函数
来源：http://bss.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://isd.daxiang520.top

PHP:  // 无泛型
来源：http://gzs.havefunace.top

JS:   // 无泛型
来源：http://pjw.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://klm.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gsy.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bgc.bjfxy.top

Ruby: # 无泛型
来源：http://bid.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cal.sysykeji.top

[C15] 解构 / 展开参数
来源：http://ksb.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sce.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://wzm.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqp.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zhl.smart0.xyz

Java: // 无解构
来源：http://ake.epnwcf.com

Go:   // 无解构
来源：http://myz.iojbl.cn

Ruby: a, b = pair
来源：http://ect.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://rvj.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://tcm.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xfm.sweek.top

PHP:  // 无重载
来源：http://iio.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fho.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://hqm.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://opq.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://iak.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://ixu.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://wxk.jiagoushi.top

================================================================================
来源：http://vtr.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://ykk.cucudq.cn

================================================================================
来源：http://uiq.meibo888.top

[D01] 创建数组 / 列表
来源：http://zgc.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cwq.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://stm.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://abg.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://iys.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xpg.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://dri.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://yji.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oro.bjfxy.top

[D02] 追加元素到末尾
来源：http://nth.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fzv.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nbv.shuidangran.top

JS:   arr.push(4);
来源：http://naf.fengsongda.top

TS:   arr.push(4);
来源：http://qam.52xcode.cn

Java: list.add(4);
来源：http://xvw.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://qnd.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ssd.yj202588.top

C#:   list.Add(4);
来源：http://nrz.pycfn.com

[D03] 在指定位置插入元素
来源：http://isi.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://xpk.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hte.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nly.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://chn.zhixingplan.top

Java: list.add(0, 0);
来源：http://imo.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iwk.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cce.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://ckj.guannengcc.top

[D04] 删除元素
来源：http://xwl.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cwh.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://akp.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dvs.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://ckf.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bnd.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pwv.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://new.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pyv.snrcjt.cn

[D05] 访问与修改元素
来源：http://fei.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pog.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bxr.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vgp.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://ylb.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://sed.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://eme.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qss.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jzm.sjlbkw.cn

[D06] 数组长度
来源：http://kzh.c1oappe.top

Py:   len(arr)
来源：http://iww.yueranfly.top

PHP:  count($arr);
来源：http://cfx.gogol.net.cn

JS:   arr.length
来源：http://lkj.gaohongyu789.top

TS:   arr.length
来源：http://tfk.fanxiaobao.xyz

Java: list.size();
来源：http://xtj.sjlbkw.cn

Go:   len(arr)
来源：http://gzp.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://xgq.gotoacloud.top

C#:   list.Count;
来源：http://lza.bjfxy.top

[D07] 切片 / 取子数组
来源：http://sep.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nup.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mof.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://anp.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://zfk.tarul.cn

Java: list.subList(1, 4);
来源：http://vbj.jlsjyb.cn

Go:   arr[1:4]
来源：http://nco.zdbjq.cn

Ruby: arr[1, 3]
来源：http://vne.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://slq.sysykeji.top

[D08] 合并两个数组
来源：http://mgf.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://rxr.meibo888.top

PHP:  array_merge($a, $b);
来源：http://ikh.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://vnm.yuxming.cn

TS:   [...a, ...b];
来源：http://vgl.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yaj.kuanghao11.cn

Go:   append(a, b...)
来源：http://mjx.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://ktc.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://xiz.jinqigufen.top

[D09] 排序（升序）
来源：http://ywb.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ram.sjlbkw.cn

PHP:  sort($arr);
来源：http://sbv.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fim.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jqj.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yih.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tkx.zdbjq.cn

Ruby: arr.sort
来源：http://nrm.quarkkingdee.top

C#:   list.Sort();
来源：http://rru.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yhf.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hqj.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvb.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jjn.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dps.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jqb.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sda.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dac.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bbr.yj20258888.top

[D11] 反转数组
来源：http://tit.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://rlo.yongpay.top

PHP:  array_reverse($arr);
来源：http://irt.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ied.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://xms.svipenyu.cn

Java: Collections.reverse(list);
来源：http://wpy.tanke756.top

Go:   slices.Reverse(arr)
来源：http://scq.daxiang520.top

Ruby: arr.reverse
来源：http://ftu.jiagoushi.top

C#:   list.Reverse();
来源：http://vtr.tian-w.cn

[D12] 查找元素下标
来源：http://orx.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://esd.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xwf.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrx.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ljj.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://esi.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://frf.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://ffy.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://wui.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://nzm.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://huu.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bny.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://yex.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://stg.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jso.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bqd.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zcr.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://mss.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://alw.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://amj.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vea.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://dxl.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://hxl.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gmy.52xcode.cn

Go:   // 手写循环
来源：http://xmt.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://juc.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://heg.daxiang520.top

[D15] 去重
来源：http://knb.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tcs.smart0.xyz

PHP:  array_unique($arr);
来源：http://cib.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://tip.mhx1999.top

TS:   [...new Set(arr)]
来源：http://syv.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jzv.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://qjx.tian-w.cn

Ruby: arr.uniq
来源：http://vkx.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://www.xuanzx.com

[D16] 求和与平均值
来源：http://zvy.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aww.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dym.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhl.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bga.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rgm.sjlbkw.cn

Go:   // 手写循环累加
来源：http://exb.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mni.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://mhp.vehdjk.com

[D17] 最大值与最小值
来源：http://vtk.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://awl.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://qtt.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fle.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://uoy.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fyc.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sgm.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://plz.ivvv.top

C#:   list.Max();  list.Min()
来源：http://coh.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://lqw.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yxh.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://ynb.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ikp.tian-w.cn

TS:   nested.flat();
来源：http://rud.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jfw.ehwqpu.com

Go:   // 手写双层循环
来源：http://hxy.gotoacloud.top

Ruby: nested.flatten
来源：http://dfp.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://eoi.ppjwa.cn

[D19] 按字段分组
来源：http://qao.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mim.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qjk.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cwt.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pta.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ruh.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://gur.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ktm.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ghl.yonumen.top

[D20] 统计每个元素出现次数
来源：http://xyk.xinyue.icu

Py:   Counter(arr)
来源：http://qow.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://bgj.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvk.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://swo.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://omh.ydzc1.top

Go:   // 手写 map[T]int
来源：http://swc.andypj.xyz

Ruby: arr.tally
来源：http://ahk.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zqm.ivvv.top

[D21] 判断是否包含某元素
来源：http://ipf.jlsjyb.cn

Py:   x in arr
来源：http://iwp.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://xvd.yongpay.top

JS:   arr.includes(x)
来源：http://wzh.ydjk.org.cn

TS:   arr.includes(x)
来源：http://syh.jinqigfzy.top

Java: list.contains(x)
来源：http://oso.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://qnb.shzxlz.cn

Ruby: arr.include?(x)
来源：http://gkk.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://msi.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://jvb.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://auz.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://raj.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uym.feifeiyinyue.top

TS:   [...arr];
来源：http://wck.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://bnv.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://tfp.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://ioa.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://quf.fzhhl.top

[D23] reduce 累积计算
来源：http://fna.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hni.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lpm.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbb.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sds.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vkr.zhixingplan.top

Go:   // 手写循环
来源：http://kca.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pjh.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mjv.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://sfo.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xec.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cgu.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://umf.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mqi.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aic.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mxz.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://arn.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uxd.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://waa.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pul.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjn.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baf.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://csk.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwc.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vlb.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://imw.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ref.andypj.xyz

[D26] 数组转字符串
来源：http://rql.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://lyk.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://ayk.9152youxi.cn

JS:   arr.join(", ")
来源：http://zdy.vqdsnc.cn

TS:   arr.join(", ")
来源：http://qkn.hammf.cn

Java: String.join(", ", list)
来源：http://omk.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://zxh.hnqzz.top

Ruby: arr.join(", ")
来源：http://jop.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://yqz.zycfv.cn

================================================================================
来源：http://okc.hesvh.cn

E. 字符串处理
来源：http://fue.birdmap.top

================================================================================
来源：http://nmv.ivvv.top

[E01] 拼接字符串
来源：http://dfw.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpp.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yrq.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vnm.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bep.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://trj.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gqk.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ach.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://phn.pycfn.com

[E02] 重复字符串
来源：http://quv.uphjek.com

Py:   "ab" * 3
来源：http://rsq.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://hcc.bjfxy.top

JS:   "ab".repeat(3)
来源：http://chl.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://qlu.jianghu66.top

Java: "ab".repeat(3)
来源：http://wsx.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://dyf.sysykeji.top

Ruby: "ab" * 3
来源：http://jqv.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ygl.daria6918.cn

[E03] 截取子串
来源：http://faq.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zyh.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kmn.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dcf.andypj.xyz

TS:   s.slice(1, 4)
来源：http://vrz.hnqzz.top

Java: s.substring(1, 4)
来源：http://pbu.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cic.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://oil.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://yks.jyoumei.cn

[E04] 查找子串位置
来源：http://hnd.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://sqa.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://jqw.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kov.jinqigufen.top

TS:   s.indexOf("x")
来源：http://lsp.yongpay.top

Java: s.indexOf("x")
来源：http://thl.nwbrower.top


<!-- 参考信息 -->