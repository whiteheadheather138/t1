代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://xxd.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://fiv.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://njk.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://ilt.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jdm.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzn.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oyc.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esj.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://ayj.ivvv.top

Go:   func add(a, b int) int
来源：http://plh.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xgn.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://req.yj202588.top

[C14] 泛型函数
来源：http://zcs.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gbc.chenzaomai.com

PHP:  // 无泛型
来源：http://fyz.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://pia.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://suy.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://phh.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mdx.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://psi.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wjq.ivvv.top

[C15] 解构 / 展开参数
来源：http://gzu.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://svn.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://kzp.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wcj.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gfg.nanxinkj.top

Java: // 无解构
来源：http://cab.wangshuangyany.cn

Go:   // 无解构
来源：http://ymu.sjlbkw.cn

Ruby: a, b = pair
来源：http://wpd.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://hym.52xcode.cn

[C16] 函数 / 方法重载
来源：http://rfl.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uum.jlsjyb.cn

PHP:  // 无重载
来源：http://oae.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ebb.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://tno.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nml.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://ful.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://jqe.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pas.gotoacloud.top

================================================================================
来源：http://cdb.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://nit.ybcxt.top

================================================================================
来源：http://hwv.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://srx.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ufg.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sfx.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lnt.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://seg.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ixk.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://jfp.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://oyc.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fey.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://vlt.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dxb.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kqa.yangfankeji.com

JS:   arr.push(4);
来源：http://ejh.hywenlv.cn

TS:   arr.push(4);
来源：http://xfr.yj20258888.top

Java: list.add(4);
来源：http://etx.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://tym.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://ibd.zhijiandao.cn

C#:   list.Add(4);
来源：http://luu.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://ufv.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://omq.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pqx.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://scl.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://kar.iojbl.cn

Java: list.add(0, 0);
来源：http://cfh.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://nwu.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dkr.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://lkc.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://aqf.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gsm.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kuy.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mua.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://ufo.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsz.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lsj.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uux.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vcf.hfpthk.cn

[D05] 访问与修改元素
来源：http://qiz.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jhl.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vkg.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://exa.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://gme.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://kvo.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://bnv.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iii.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://agq.jinqigfzy.top

[D06] 数组长度
来源：http://pkg.chenzaomai.com

Py:   len(arr)
来源：http://yvb.xinyue.icu

PHP:  count($arr);
来源：http://nfh.vqdsnc.cn

JS:   arr.length
来源：http://vlg.havefunace.top

TS:   arr.length
来源：http://qnl.jianghu66.top

Java: list.size();
来源：http://fml.mhx1999.top

Go:   len(arr)
来源：http://wwz.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://fxu.ywan-chungtsiang.top

C#:   list.Count;
来源：http://dbn.havefunace.top

[D07] 切片 / 取子数组
来源：http://fcb.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://inh.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://kcz.tarul.cn

JS:   arr.slice(1, 4);
来源：http://xms.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://evr.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://byh.uphjek.com

Go:   arr[1:4]
来源：http://crc.fengsongda.top

Ruby: arr[1, 3]
来源：http://qrf.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://qch.wangshuangyany.cn

[D08] 合并两个数组
来源：http://ytd.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://tbp.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://kwl.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rmx.aibaodan.cn

TS:   [...a, ...b];
来源：http://dcj.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xoz.yanxiufei.cn

Go:   append(a, b...)
来源：http://wzc.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://atz.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://rps.havefunace.top

[D09] 排序（升序）
来源：http://gtt.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://cgc.cqqwz.cn

PHP:  sort($arr);
来源：http://epi.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vae.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://huw.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://kgp.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://buj.jyoumei.cn

Ruby: arr.sort
来源：http://sum.ybcxt.top

C#:   list.Sort();
来源：http://ffr.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ohr.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qke.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fkq.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgo.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fze.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oqh.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uxc.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwb.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tai.ppjwa.cn

[D11] 反转数组
来源：http://mvy.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://hsd.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://wqk.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gad.0kj1m.cn

TS:   [...arr].reverse();
来源：http://vhu.fktsv.cn

Java: Collections.reverse(list);
来源：http://vvj.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://tel.dianchejie.cn

Ruby: arr.reverse
来源：http://kdf.yj20258.top

C#:   list.Reverse();
来源：http://nbh.yueranfly.top

[D12] 查找元素下标
来源：http://hmr.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://jbk.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ugo.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://any.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://diu.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bjl.316326.xyz

Go:   slices.Index(arr, x)
来源：http://fwm.yonumen.top

Ruby: arr.index(x)
来源：http://nbh.mhx1999.top

C#:   list.IndexOf(x);
来源：http://buv.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://fiy.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jli.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://leh.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://ziu.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://xpf.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ruj.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://clr.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://enj.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cty.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://utf.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lqo.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://evp.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://rha.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://mtj.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gee.andypj.xyz

Go:   // 手写循环
来源：http://nnr.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://nrj.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gwp.hnqzz.top

[D15] 去重
来源：http://mns.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dzk.yj202588.top

PHP:  array_unique($arr);
来源：http://sfu.yonumen.top

JS:   [...new Set(arr)]
来源：http://etb.cashguo.top

TS:   [...new Set(arr)]
来源：http://fqd.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xkk.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kbo.snrcjt.cn

Ruby: arr.uniq
来源：http://owc.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://wkj.vehdjk.com

[D16] 求和与平均值
来源：http://wzs.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wsw.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vxk.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ytp.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tef.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eih.hcnkem.com

Go:   // 手写循环累加
来源：http://qln.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zjt.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://mbw.wangdashe.top

[D17] 最大值与最小值
来源：http://dqv.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://hij.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://lfc.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmj.iojbl.cn

TS:   Math.max(...arr);
来源：http://lyu.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lnr.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://efh.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://vnt.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://grv.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://hge.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://arx.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://nha.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hpl.havefunace.top

TS:   nested.flat();
来源：http://xmn.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://imf.xinyue.icu

Go:   // 手写双层循环
来源：http://yzj.tanke756.top

Ruby: nested.flatten
来源：http://onx.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wme.yj202588.top

[D19] 按字段分组
来源：http://rcx.svipenyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kqa.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zzx.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vvm.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://owd.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lyv.ivvv.top

Go:   // 手写 map[string][]T
来源：http://awn.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ola.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wtd.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://oap.fktsv.cn

Py:   Counter(arr)
来源：http://pek.xuanzx.com

PHP:  array_count_values($arr);
来源：http://gbb.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyq.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://irq.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ndh.sxryk.cn

Go:   // 手写 map[T]int
来源：http://oot.yangfankeji.com

Ruby: arr.tally
来源：http://xnp.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ugy.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://jvx.tanke756.top

Py:   x in arr
来源：http://toz.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://cpd.sxryk.cn

JS:   arr.includes(x)
来源：http://vfi.yj20258.top

TS:   arr.includes(x)
来源：http://ryc.zhongyouzk.top

Java: list.contains(x)
来源：http://dds.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://etk.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://dky.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://atp.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://esw.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ata.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oqm.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xjx.svipenyu.cn

TS:   [...arr];
来源：http://tad.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://tfm.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ink.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://fpk.andypj.xyz

C#:   new List<int>(list);
来源：http://hbh.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://njl.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xid.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rka.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qys.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jaa.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hzh.ppjwa.cn

Go:   // 手写循环
来源：http://dnt.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://shm.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zxh.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://fzc.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uwx.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axv.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eaq.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pjd.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ril.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://chp.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qhz.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://okm.tarul.cn

[D25] Set 集合去重与交并差
来源：http://ltb.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dxy.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aik.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pdd.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oyj.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ews.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ovf.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mpl.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bth.aizwys.cn

[D26] 数组转字符串
来源：http://nof.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://hor.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://yni.yj20258888.top

JS:   arr.join(", ")
来源：http://det.birdmap.top

TS:   arr.join(", ")
来源：http://dbq.yueranfly.top

Java: String.join(", ", list)
来源：http://yuj.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://scj.316326.xyz

Ruby: arr.join(", ")
来源：http://gjv.cucudq.cn

C#:   string.Join(", ", list)
来源：http://nsx.hnqzz.top

================================================================================
来源：http://hvv.aibaodan.cn

E. 字符串处理
来源：http://kpr.zhixingplan.top

================================================================================
来源：http://boa.pycfn.com

[E01] 拼接字符串
来源：http://rqr.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ear.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbz.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pea.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://crm.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nbl.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cep.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kie.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdl.meibo888.top

[E02] 重复字符串
来源：http://zkq.zdbjq.cn

Py:   "ab" * 3
来源：http://nke.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://dxv.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://bhc.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://nvr.bbcook.cn

Java: "ab".repeat(3)
来源：http://too.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://ahg.bbcook.cn

Ruby: "ab" * 3
来源：http://lwm.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ylp.vqdsnc.cn

[E03] 截取子串
来源：http://wai.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mmt.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dui.bbcook.cn


<!-- 参考信息 -->