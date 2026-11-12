代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://liz.fengsongda.top

Go:   func add(a, b int) int
来源：http://ffi.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dfg.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://urj.nanxuanxn.top

[C14] 泛型函数
来源：http://aty.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ihc.guowangkeji.top

PHP:  // 无泛型
来源：http://yse.sufxvd.cn

JS:   // 无泛型
来源：http://wdo.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mhp.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pmq.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sbl.fengsongda.top

Ruby: # 无泛型
来源：http://tda.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wgg.c1oappe.top

[C15] 解构 / 展开参数
来源：http://qvq.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ufq.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://kbp.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hkv.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ufd.jlsjyb.cn

Java: // 无解构
来源：http://jez.ctjpmb.com

Go:   // 无解构
来源：http://pam.daxiang520.top

Ruby: a, b = pair
来源：http://hwt.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://lra.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://fxt.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fsg.hnqzz.top

PHP:  // 无重载
来源：http://pvv.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://idp.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://qsp.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dvv.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://axh.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://ssn.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://byj.redwolf501.top

================================================================================
来源：http://kxc.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://npz.aibaodan.cn

================================================================================
来源：http://xud.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://wnw.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://stm.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hnq.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbc.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzv.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzu.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://gor.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://goq.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hkj.hfpthk.cn

[D02] 追加元素到末尾
来源：http://wnr.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xan.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ynt.cashguo.top

JS:   arr.push(4);
来源：http://abe.yj20258888.top

TS:   arr.push(4);
来源：http://tgy.zdbjq.cn

Java: list.add(4);
来源：http://dfn.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://lzi.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://tmj.ybcxt.top

C#:   list.Add(4);
来源：http://crh.xylfe.cn

[D03] 在指定位置插入元素
来源：http://mgb.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://zsv.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdt.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cqm.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://knf.cdnleiting.top

Java: list.add(0, 0);
来源：http://pin.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://fac.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://atz.tanke756.top

C#:   list.Insert(0, 0);
来源：http://abg.hnxiangtu.top

[D04] 删除元素
来源：http://bsx.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://icd.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oth.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ydq.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://gsu.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uhf.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://apa.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ytl.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pww.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://hqq.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xbo.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lkb.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fvu.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://fkn.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://ppp.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://rey.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://alh.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nda.shanyushiyangkeji.top

[D06] 数组长度
来源：http://ggu.fzhhl.top

Py:   len(arr)
来源：http://lih.svipenyu.cn

PHP:  count($arr);
来源：http://iij.ywan-chungtsiang.top

JS:   arr.length
来源：http://ouh.chenlongwang.top

TS:   arr.length
来源：http://jtd.jiagoushi.top

Java: list.size();
来源：http://qyw.daria6918.cn

Go:   len(arr)
来源：http://efw.yj20258.top

Ruby: arr.length; arr.size
来源：http://wzu.wangdashe.top

C#:   list.Count;
来源：http://rhz.pycfn.com

[D07] 切片 / 取子数组
来源：http://aqv.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ezu.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://ugz.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://ldh.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://mec.nanxinkj.top

Java: list.subList(1, 4);
来源：http://tbl.9152youxi.cn

Go:   arr[1:4]
来源：http://cuq.ivvv.top

Ruby: arr[1, 3]
来源：http://cmg.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://trj.tian-w.cn

[D08] 合并两个数组
来源：http://rxa.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://zfj.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://rnu.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nbm.vehdjk.com

TS:   [...a, ...b];
来源：http://qut.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gzr.svipenyu.cn

Go:   append(a, b...)
来源：http://qfg.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://zaf.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://ind.ctjpmb.com

[D09] 排序（升序）
来源：http://nzx.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://slu.fktsv.cn

PHP:  sort($arr);
来源：http://amu.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wcc.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://voo.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qpf.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlu.shzxlz.cn

Ruby: arr.sort
来源：http://hub.ydjk.org.cn

C#:   list.Sort();
来源：http://jtc.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lio.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ber.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kni.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uod.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://etg.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vxc.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bhh.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jrs.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ool.snrcjt.cn

[D11] 反转数组
来源：http://pba.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nnk.yonumen.top

PHP:  array_reverse($arr);
来源：http://erh.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zab.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://rqc.yuxming.cn

Java: Collections.reverse(list);
来源：http://jtx.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://fon.birdmap.top

Ruby: arr.reverse
来源：http://gpc.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://osp.hfpthk.cn

[D12] 查找元素下标
来源：http://inz.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://xzs.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vtz.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grc.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bra.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xrl.yongpay.top

Go:   slices.Index(arr, x)
来源：http://lns.jqgfzy.top

Ruby: arr.index(x)
来源：http://cad.yueranfly.top

C#:   list.IndexOf(x);
来源：http://uaj.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://wca.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zwa.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nye.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://dzn.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://sbw.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jdc.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yce.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://nid.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vuz.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://ezr.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qml.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://slb.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://dyt.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://jfz.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bkg.c1oappe.top

Go:   // 手写循环
来源：http://xex.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://zgw.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://okw.nanxinkj.top

[D15] 去重
来源：http://sgm.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oma.ehwqpu.com

PHP:  array_unique($arr);
来源：http://uax.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://wfu.c1oappe.top

TS:   [...new Set(arr)]
来源：http://cfa.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fxq.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://tci.shuidangran.top

Ruby: arr.uniq
来源：http://naa.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://weo.dashuyun.cn

[D16] 求和与平均值
来源：http://dat.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ubi.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rcm.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqp.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmw.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jqu.ehwqpu.com

Go:   // 手写循环累加
来源：http://qqb.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bnb.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://gqt.fengsongda.top

[D17] 最大值与最小值
来源：http://yct.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://fkp.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://hyc.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xtv.zdqjudy.top

TS:   Math.max(...arr);
来源：http://hhy.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vhx.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dqd.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://kck.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://gvx.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://xre.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://isq.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://kbx.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kwp.zhixingplan.top

TS:   nested.flat();
来源：http://svv.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://adz.zdqjudy.top

Go:   // 手写双层循环
来源：http://xdi.9152youxi.cn

Ruby: nested.flatten
来源：http://ffk.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dwn.xziqi.cn

[D19] 按字段分组
来源：http://xwd.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbm.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yuy.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rgr.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hdl.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nto.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://cax.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dby.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gva.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://gjt.yj202588.top

Py:   Counter(arr)
来源：http://sfd.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://lex.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwh.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzs.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cks.fehbvm.com

Go:   // 手写 map[T]int
来源：http://mnu.redwolf501.top

Ruby: arr.tally
来源：http://wsv.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ess.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://cms.pycfn.com

Py:   x in arr
来源：http://rqr.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://nwl.sufxvd.cn

JS:   arr.includes(x)
来源：http://jws.ydzc1.top

TS:   arr.includes(x)
来源：http://fpq.jlsjyb.cn

Java: list.contains(x)
来源：http://yjg.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://doy.yangfankeji.com

Ruby: arr.include?(x)
来源：http://rfj.sufxvd.cn

C#:   list.Contains(x)
来源：http://wxp.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://unr.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vjx.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ahx.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jtd.fzhhl.top

TS:   [...arr];
来源：http://tre.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://ahb.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dmz.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://xwm.chenzaomai.com

C#:   new List<int>(list);
来源：http://tho.yvedp.cn

[D23] reduce 累积计算
来源：http://dlp.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://csl.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lxk.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffw.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vir.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rzq.daxiang520.top

Go:   // 手写循环
来源：http://gqf.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aer.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgg.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://uvr.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cbz.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sbr.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sfq.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hab.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ifm.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dcw.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aqy.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyl.hammf.cn

[D25] Set 集合去重与交并差
来源：http://pge.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://npr.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gmh.0kj1m.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hqn.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bcn.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ggu.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://seg.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hgd.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://umw.yangfankeji.com

[D26] 数组转字符串
来源：http://lgh.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://pxb.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://zgn.jqgfzy.top

JS:   arr.join(", ")
来源：http://aox.yonumen.top

TS:   arr.join(", ")
来源：http://tgy.fehbvm.com

Java: String.join(", ", list)
来源：http://veg.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://zec.hfpthk.cn

Ruby: arr.join(", ")
来源：http://omq.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://vby.sjlbkw.cn

================================================================================
来源：http://jcd.zhixingplan.top

E. 字符串处理
来源：http://cxt.cdnleiting.top

================================================================================
来源：http://mhp.bjfxy.top

[E01] 拼接字符串
来源：http://kng.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kmj.vqdsnc.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ymw.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qve.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zmp.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yku.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gyb.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qve.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ack.zhiwuduotai.top

[E02] 重复字符串
来源：http://fca.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://kkb.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://dpx.fktsv.cn

JS:   "ab".repeat(3)
来源：http://rqh.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://vqw.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://vjp.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://gxg.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://cfu.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fon.chenlongwang.top

[E03] 截取子串
来源：http://rbd.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vqs.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihy.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dex.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://guy.sxryk.cn

Java: s.substring(1, 4)
来源：http://qge.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yaf.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://fmf.havefunace.top

C#:   s.Substring(1, 3)
来源：http://vtm.ctjpmb.com

[E04] 查找子串位置
来源：http://dke.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://hxj.xingfuxueyuan.xyz


<!-- 参考信息 -->