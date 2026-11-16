代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ikc.daria6918.cn

Go:   func add(a, b int) int
来源：http://xfs.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cvv.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iqd.zdqjudy.top

[C14] 泛型函数
来源：http://oli.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cce.0kj1m.cn

PHP:  // 无泛型
来源：http://oun.yonumen.top

JS:   // 无泛型
来源：http://jhu.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dls.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fqn.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ble.c1oappe.top

Ruby: # 无泛型
来源：http://mor.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bxe.smart0.xyz

[C15] 解构 / 展开参数
来源：http://ges.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rmx.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://hlq.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://njx.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tsj.jyoumei.cn

Java: // 无解构
来源：http://qnc.yueranfly.top

Go:   // 无解构
来源：http://cnc.yuxming.cn

Ruby: a, b = pair
来源：http://tah.nwbrower.top

C#:   var (a, b) = pair;
来源：http://etb.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://unw.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mom.zdqjudy.top

PHP:  // 无重载
来源：http://tyh.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bud.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://dqu.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://flx.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://orf.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://dte.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://qrp.jinqigufen.top

================================================================================
来源：http://fqw.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://oip.316326.xyz

================================================================================
来源：http://rsi.bbcook.cn

[D01] 创建数组 / 列表
来源：http://ewh.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bbd.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rzd.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nmc.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bpt.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://muz.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://omt.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://jcl.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofy.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://fpz.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kdu.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sgk.jiagoushi.top

JS:   arr.push(4);
来源：http://wep.vqdsnc.cn

TS:   arr.push(4);
来源：http://jdz.hnxiangtu.top

Java: list.add(4);
来源：http://jnw.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://nkf.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://tjy.yonumen.top

C#:   list.Add(4);
来源：http://ioc.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://vao.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://zty.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://isw.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgr.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://xcf.zhongyouzk.top

Java: list.add(0, 0);
来源：http://efk.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kid.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tne.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://vav.shangyingyoupin.top

[D04] 删除元素
来源：http://lyb.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hut.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kwl.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xtn.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://xxi.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jzz.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vod.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cdi.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://crn.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://nfm.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vpl.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://edp.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zav.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://lau.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://qtm.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://lge.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wgl.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kga.daria6918.cn

[D06] 数组长度
来源：http://kkz.svipenyu.cn

Py:   len(arr)
来源：http://enq.yonumen.top

PHP:  count($arr);
来源：http://hhy.pengpengdd.cyou

JS:   arr.length
来源：http://tur.hcnkem.com

TS:   arr.length
来源：http://koj.zycfv.cn

Java: list.size();
来源：http://kip.jiagoushi.top

Go:   len(arr)
来源：http://giw.xuanzx.com

Ruby: arr.length; arr.size
来源：http://pzr.sufxvd.cn

C#:   list.Count;
来源：http://qtm.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://dpz.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://phh.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://apt.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://nqq.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://iyk.jinqigufen.top

Java: list.subList(1, 4);
来源：http://ysg.nanxuanxn.top

Go:   arr[1:4]
来源：http://wmg.wangdashe.top

Ruby: arr[1, 3]
来源：http://tfn.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://ddc.yongpay.top

[D08] 合并两个数组
来源：http://mub.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://ybd.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://vby.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://chx.guannengcc.top

TS:   [...a, ...b];
来源：http://zvh.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fou.ehwqpu.com

Go:   append(a, b...)
来源：http://wkd.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://arr.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://erm.haohaochexian.top

[D09] 排序（升序）
来源：http://pmm.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://fnt.hysaishi.cn

PHP:  sort($arr);
来源：http://jkq.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gwf.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://dbu.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qef.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pci.zhoulong.xyz

Ruby: arr.sort
来源：http://gkc.jinqigufen.top

C#:   list.Sort();
来源：http://wls.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://blt.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mvn.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzo.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rmu.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pga.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ten.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tvi.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dka.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tby.hammf.cn

[D11] 反转数组
来源：http://pnh.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://xfh.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://cew.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ozu.yuxming.cn

TS:   [...arr].reverse();
来源：http://zbl.xylfe.cn

Java: Collections.reverse(list);
来源：http://vlk.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://nhu.uphjek.com

Ruby: arr.reverse
来源：http://yug.sjlbkw.cn

C#:   list.Reverse();
来源：http://kjw.zhengqikj.top

[D12] 查找元素下标
来源：http://fwh.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://pny.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qwg.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tst.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fco.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://typ.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://ire.316326.xyz

Ruby: arr.index(x)
来源：http://dxk.316326.xyz

C#:   list.IndexOf(x);
来源：http://cvt.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://kfc.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tgu.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://whf.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://gxy.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://eid.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://amh.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fyr.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://siq.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qlv.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://ntm.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zrm.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yyf.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://hpk.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://ewk.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zpq.sxryk.cn

Go:   // 手写循环
来源：http://dav.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lug.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://grg.pycfn.com

[D15] 去重
来源：http://jra.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ybp.xinyue.icu

PHP:  array_unique($arr);
来源：http://sut.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://ocv.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://eux.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ira.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://sbc.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://kln.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://rdz.pengpengdd.cyou

[D16] 求和与平均值
来源：http://xon.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jjz.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dnc.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qxs.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://upk.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bjf.yj20258888.top

Go:   // 手写循环累加
来源：http://htr.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ldf.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://kak.iojbl.cn

[D17] 最大值与最小值
来源：http://siq.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://znb.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://oti.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nsb.hywenlv.cn

TS:   Math.max(...arr);
来源：http://csl.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eqh.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kdx.yongpay.top

Ruby: arr.max;  arr.min
来源：http://kpj.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://lty.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://zvt.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lxo.tanke756.top

PHP:  array_merge(...$nested);
来源：http://nvj.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pau.yuxming.cn

TS:   nested.flat();
来源：http://tix.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wey.hcnkem.com

Go:   // 手写双层循环
来源：http://qqy.havefunace.top

Ruby: nested.flatten
来源：http://zwb.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wqb.shanyushiyangtech.top

[D19] 按字段分组
来源：http://yfi.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://obc.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xse.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mpu.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vem.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aix.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://tam.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qwd.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zve.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://vhn.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://dyk.cashguo.top

PHP:  array_count_values($arr);
来源：http://hmd.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prd.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kkz.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uzy.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://hav.yj20258.top

Ruby: arr.tally
来源：http://ubp.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jxp.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://nkx.zycfv.cn

Py:   x in arr
来源：http://ugi.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://cyb.yuxming.cn

JS:   arr.includes(x)
来源：http://wcu.redwolf501.top

TS:   arr.includes(x)
来源：http://pkj.sjlbkw.cn

Java: list.contains(x)
来源：http://mqy.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://wfr.cucudq.cn

Ruby: arr.include?(x)
来源：http://ycp.zycfv.cn

C#:   list.Contains(x)
来源：http://rvd.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://ypf.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://omy.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rok.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ovi.wangshuangyany.cn

TS:   [...arr];
来源：http://fro.c1oappe.top

Java: new ArrayList<>(list);
来源：http://usm.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://mao.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://ouc.yonumen.top

C#:   new List<int>(list);
来源：http://oml.zycfv.cn

[D23] reduce 累积计算
来源：http://sjm.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pcc.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kjf.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkv.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://agk.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vng.hammf.cn

Go:   // 手写循环
来源：http://dkp.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfi.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wuz.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://hgw.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xex.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://loo.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lzc.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dbs.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tmj.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://raa.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://luh.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gwg.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://ciz.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tjt.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://duv.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cgg.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dmf.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dhw.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uaz.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rok.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dvo.quarkkingdee.top

[D26] 数组转字符串
来源：http://qht.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://oez.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://dsy.shuidangran.top

JS:   arr.join(", ")
来源：http://wvb.cdnleiting.top

TS:   arr.join(", ")
来源：http://ilf.ydjk.org.cn

Java: String.join(", ", list)
来源：http://obc.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://nzy.0kj1m.cn

Ruby: arr.join(", ")
来源：http://vhe.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://woj.shuidangran.top

================================================================================
来源：http://rlv.hywenlv.cn

E. 字符串处理
来源：http://znm.zhaomingkeji.xyz

================================================================================
来源：http://hum.zhoulong.xyz

[E01] 拼接字符串
来源：http://pyt.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vpo.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fcv.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wnv.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cig.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qpi.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rut.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://smw.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dts.vqdsnc.cn

[E02] 重复字符串
来源：http://por.9152youxi.cn

Py:   "ab" * 3
来源：http://kkd.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://sfp.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://ich.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://kbw.fzhhl.top

Java: "ab".repeat(3)
来源：http://nyv.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://btr.jqgfzy.top

Ruby: "ab" * 3
来源：http://hip.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rsx.xziqi.cn

[E03] 截取子串
来源：http://xbf.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://erg.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ttm.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zvu.hnqzz.top

TS:   s.slice(1, 4)
来源：http://jcg.yuxming.cn

Java: s.substring(1, 4)
来源：http://rjd.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://npw.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kor.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://epl.zdbjq.cn

[E04] 查找子串位置
来源：http://qrp.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://luz.yanxiufei.cn


<!-- 参考信息 -->