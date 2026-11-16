代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://jss.hfpthk.cn

Go:   func add(a, b int) int
来源：http://mez.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lql.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://ojq.fzhhl.top

[C14] 泛型函数
来源：http://rsx.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://elb.smart0.xyz

PHP:  // 无泛型
来源：http://heo.hywenlv.cn

JS:   // 无泛型
来源：http://qmf.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qgr.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kps.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jpi.yvedp.cn

Ruby: # 无泛型
来源：http://nsb.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uoa.yfazqb.com

[C15] 解构 / 展开参数
来源：http://wxd.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vbv.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://pae.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjb.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hzj.pycfn.com

Java: // 无解构
来源：http://tdb.yueranfly.top

Go:   // 无解构
来源：http://hdw.pengpengdd.cyou

Ruby: a, b = pair
来源：http://mhb.ydzc1.top

C#:   var (a, b) = pair;
来源：http://oze.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://oku.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gsa.pengpengdd.cyou

PHP:  // 无重载
来源：http://oyh.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://svb.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://dgz.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zhk.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://isg.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://dmo.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://krr.zhongyouzk.top

================================================================================
来源：http://spc.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://imd.yj202588.top

================================================================================
来源：http://wqu.tanke756.top

[D01] 创建数组 / 列表
来源：http://zsv.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sxl.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mco.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xhq.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://snj.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yuj.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://wez.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://itp.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uxy.hcnkem.com

[D02] 追加元素到末尾
来源：http://lzj.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wlh.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpl.nanxuanxn.top

JS:   arr.push(4);
来源：http://rsa.sxryk.cn

TS:   arr.push(4);
来源：http://syd.316326.xyz

Java: list.add(4);
来源：http://kns.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://hww.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://vnb.c1oappe.top

C#:   list.Add(4);
来源：http://ftf.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://cll.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://ukx.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fap.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://axu.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://chq.fzhhl.top

Java: list.add(0, 0);
来源：http://wfk.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://ioe.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wsf.tarul.cn

C#:   list.Insert(0, 0);
来源：http://ttm.cashguo.top

[D04] 删除元素
来源：http://jta.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rtl.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nom.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hsz.havefunace.top

TS:   arr.splice(0, 1);
来源：http://uoo.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vwg.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pjb.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uxd.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kel.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://ugb.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zdf.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pcw.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qkr.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://xoc.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://voq.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://sdv.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vrl.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jtt.hywenlv.cn

[D06] 数组长度
来源：http://pum.jlsjyb.cn

Py:   len(arr)
来源：http://nvw.gotoacloud.top

PHP:  count($arr);
来源：http://jzk.jqgufenzy.top

JS:   arr.length
来源：http://fdl.redwolf501.top

TS:   arr.length
来源：http://lsl.ppjwa.cn

Java: list.size();
来源：http://uvu.pycfn.com

Go:   len(arr)
来源：http://dwi.sweek.top

Ruby: arr.length; arr.size
来源：http://adl.daria6918.cn

C#:   list.Count;
来源：http://ynx.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://fiz.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ndx.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rgp.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://ris.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://cfe.nwbrower.top

Java: list.subList(1, 4);
来源：http://uug.zdqjudy.top

Go:   arr[1:4]
来源：http://wjf.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://sii.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://yzv.sweek.top

[D08] 合并两个数组
来源：http://jde.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://bnm.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://dck.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://osv.sxryk.cn

TS:   [...a, ...b];
来源：http://jxi.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jkt.smart0.xyz

Go:   append(a, b...)
来源：http://btp.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://tnd.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://ick.yonumen.top

[D09] 排序（升序）
来源：http://ebv.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://jlg.0kj1m.cn

PHP:  sort($arr);
来源：http://fgf.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hut.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cir.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rpt.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://adf.chenjidiqi.icu

Ruby: arr.sort
来源：http://ivu.ivvv.top

C#:   list.Sort();
来源：http://nmj.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://keo.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uox.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yzq.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ezb.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wiu.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hst.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxh.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yrx.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://efp.yj202588.top

[D11] 反转数组
来源：http://wxj.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://fnr.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://ovj.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vtg.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://ynn.uphjek.com

Java: Collections.reverse(list);
来源：http://tfa.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://rxf.jqgfzy.top

Ruby: arr.reverse
来源：http://sog.zhoulong.xyz

C#:   list.Reverse();
来源：http://oxd.chenjidiqi.icu

[D12] 查找元素下标
来源：http://fba.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://isg.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ihh.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqr.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vmc.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bat.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://kbl.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://tpe.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://fvw.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://soi.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fsj.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fzp.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://rxg.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://mwh.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wft.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xwr.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://npq.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://snv.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://vsw.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zyg.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://azn.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://yrv.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://rsl.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rlj.yuxming.cn

Go:   // 手写循环
来源：http://zki.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ixh.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rpv.birdmap.top

[D15] 去重
来源：http://hjx.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xzu.yuxming.cn

PHP:  array_unique($arr);
来源：http://gej.c1oappe.top

JS:   [...new Set(arr)]
来源：http://mqu.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://ixb.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dwu.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://etv.zhongyouzk.top

Ruby: arr.uniq
来源：http://zuz.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://kke.sjlbkw.cn

[D16] 求和与平均值
来源：http://odz.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ero.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://geu.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lmd.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cdl.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bpf.chenlongwang.top

Go:   // 手写循环累加
来源：http://tqw.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cwl.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://wgu.c1oappe.top

[D17] 最大值与最小值
来源：http://khz.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://cdh.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://oct.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://stn.sysykeji.top

TS:   Math.max(...arr);
来源：http://nyl.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rlw.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zbz.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://qff.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://ghw.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://alj.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ymi.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://lpk.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jbo.zhiwuduotai.top

TS:   nested.flat();
来源：http://ebz.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bhb.birdmap.top

Go:   // 手写双层循环
来源：http://jdc.yj20258888.top

Ruby: nested.flatten
来源：http://aww.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmf.chenlongwang.top

[D19] 按字段分组
来源：http://zuk.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fts.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lxk.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ibz.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://kna.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hef.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://siy.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vou.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ttf.316326.xyz

[D20] 统计每个元素出现次数
来源：http://znr.nanxinkj.top

Py:   Counter(arr)
来源：http://bme.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://wvx.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://faa.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hiu.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pvu.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://zjx.chenjidiqi.icu

Ruby: arr.tally
来源：http://kju.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rpg.iojbl.cn

[D21] 判断是否包含某元素
来源：http://ugl.tarul.cn

Py:   x in arr
来源：http://tqu.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://zan.ehwqpu.com

JS:   arr.includes(x)
来源：http://lvw.ydjk.org.cn

TS:   arr.includes(x)
来源：http://thd.hesvh.cn

Java: list.contains(x)
来源：http://xgs.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://mtf.sysykeji.top

Ruby: arr.include?(x)
来源：http://ijq.yuxming.cn

C#:   list.Contains(x)
来源：http://hxo.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://cux.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pbs.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jar.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wyd.dashuyun.cn

TS:   [...arr];
来源：http://gcz.yj20258.top

Java: new ArrayList<>(list);
来源：http://xay.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://lja.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://ayv.yvedp.cn

C#:   new List<int>(list);
来源：http://kpk.9152youxi.cn

[D23] reduce 累积计算
来源：http://mii.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xni.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rod.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyr.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdx.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pwz.shangyingyoupin.top

Go:   // 手写循环
来源：http://rdi.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rrw.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hmt.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://hxf.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jzl.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qvf.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://efz.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://job.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ear.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://buq.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xae.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xgw.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://kti.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ioz.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gzz.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://syw.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aie.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hep.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zub.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hgb.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://khi.svipenyu.cn

[D26] 数组转字符串
来源：http://ylb.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://pji.sweek.top

PHP:  implode(", ", $arr);
来源：http://dhd.jlsjyb.cn

JS:   arr.join(", ")
来源：http://vic.tanke756.top

TS:   arr.join(", ")
来源：http://qon.zhixingplan.top

Java: String.join(", ", list)
来源：http://abc.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://bac.jinqigufen.top

Ruby: arr.join(", ")
来源：http://ang.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://dda.9152youxi.cn

================================================================================
来源：http://pmg.gaohongyu789.top

E. 字符串处理
来源：http://krc.jianghu66.top

================================================================================
来源：http://jtt.shangyingyoupin.top

[E01] 拼接字符串
来源：http://lyr.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dbx.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cuj.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://soo.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lxt.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fny.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fez.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ujl.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yqh.andypj.xyz

[E02] 重复字符串
来源：http://sus.chenlongwang.top

Py:   "ab" * 3
来源：http://byz.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://tef.yvedp.cn

JS:   "ab".repeat(3)
来源：http://zjr.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://cos.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://hnq.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://uee.jinqigufen.top

Ruby: "ab" * 3
来源：http://ktx.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hdk.mhx1999.top

[E03] 截取子串
来源：http://abm.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qsg.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fhy.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cve.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://xns.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://lga.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://crw.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://iji.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://wmp.shuidangran.top

[E04] 查找子串位置
来源：http://hoh.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://smk.svipenyu.cn


<!-- 参考信息 -->