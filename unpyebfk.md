代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ujq.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hba.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dsx.birdmap.top

Ruby: # 无泛型
来源：http://ubh.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qaj.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://tsf.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jft.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://mxf.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://osk.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tjy.fktsv.cn

Java: // 无解构
来源：http://viy.haohaochexian.top

Go:   // 无解构
来源：http://efw.chenlongwang.top

Ruby: a, b = pair
来源：http://kqq.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://mys.vehdjk.com

[C16] 函数 / 方法重载
来源：http://ylo.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jcb.jinqigufen.top

PHP:  // 无重载
来源：http://oby.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yek.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://rot.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://osy.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://hfg.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://xuw.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rxr.zhijiandao.cn

================================================================================
来源：http://ayl.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://xpo.yueranfly.top

================================================================================
来源：http://fea.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://uby.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jbb.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fxr.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iax.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rlu.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ghq.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://lla.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://fyb.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://krw.shzxlz.cn

[D02] 追加元素到末尾
来源：http://hrs.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lua.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozg.jinqigfzy.top

JS:   arr.push(4);
来源：http://kvq.zhixingplan.top

TS:   arr.push(4);
来源：http://vsl.svipenyu.cn

Java: list.add(4);
来源：http://sgz.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://rxx.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://pxy.yueranfly.top

C#:   list.Add(4);
来源：http://jdr.fktsv.cn

[D03] 在指定位置插入元素
来源：http://ygz.cheryme.top

Py:   arr.insert(0, 0)
来源：http://zim.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bto.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npe.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://irv.fengsongda.top

Java: list.add(0, 0);
来源：http://xpe.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://vaw.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mow.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://vdh.smart0.xyz

[D04] 删除元素
来源：http://tfh.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://igu.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vgr.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xiu.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://gqs.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rdb.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yoa.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kzp.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tim.xuanzx.com

[D05] 访问与修改元素
来源：http://tzx.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hzo.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cxp.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xur.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://nrz.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://yzj.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://ozy.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lqr.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mvl.jiagoushi.top

[D06] 数组长度
来源：http://oez.wangshuangyany.cn

Py:   len(arr)
来源：http://wjn.zhengqikj.top

PHP:  count($arr);
来源：http://mwv.hnqzz.top

JS:   arr.length
来源：http://omb.jqgufenzy.top

TS:   arr.length
来源：http://quw.zdqjudy.top

Java: list.size();
来源：http://srb.zhijiandao.cn

Go:   len(arr)
来源：http://chc.yonumen.top

Ruby: arr.length; arr.size
来源：http://ygd.vqdsnc.cn

C#:   list.Count;
来源：http://tci.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://xuj.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xel.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://egg.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://zwi.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://nbw.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://rrd.aibaodan.cn

Go:   arr[1:4]
来源：http://mob.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://ivk.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://llz.yangfankeji.com

[D08] 合并两个数组
来源：http://pxm.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://aqs.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://emw.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oji.chenlongwang.top

TS:   [...a, ...b];
来源：http://hyp.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ljo.jinqigfzy.top

Go:   append(a, b...)
来源：http://www.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://vlq.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://qdl.hcnkem.com

[D09] 排序（升序）
来源：http://azz.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://toz.tianlin.xyz

PHP:  sort($arr);
来源：http://dwe.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://syn.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fbg.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://moo.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gkt.jinqigufen.top

Ruby: arr.sort
来源：http://lev.zhoulong.xyz

C#:   list.Sort();
来源：http://csr.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqn.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vyz.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dem.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://peg.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ooe.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://taj.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mbq.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qdr.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jvv.tian-w.cn

[D11] 反转数组
来源：http://tdi.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://rao.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://wuo.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aga.yangfankeji.com

TS:   [...arr].reverse();
来源：http://zom.guowangkeji.top

Java: Collections.reverse(list);
来源：http://rvh.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://wla.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://qjj.xinyue.icu

C#:   list.Reverse();
来源：http://iqw.zdqjudy.top

[D12] 查找元素下标
来源：http://rvp.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://wwr.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dpb.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocr.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjg.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cqb.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://blg.sjlbkw.cn

Ruby: arr.index(x)
来源：http://xyg.fehbvm.com

C#:   list.IndexOf(x);
来源：http://oed.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://vyh.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aum.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://knt.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://owp.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://bqg.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xcw.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dou.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gor.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://haq.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://xkn.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lrv.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rrb.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://pln.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://nqb.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pmd.ivvv.top

Go:   // 手写循环
来源：http://dor.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lsm.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kgb.iojbl.cn

[D15] 去重
来源：http://kwq.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zfn.xylfe.cn

PHP:  array_unique($arr);
来源：http://zuh.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://sxs.fktsv.cn

TS:   [...new Set(arr)]
来源：http://uwk.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wug.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tli.hnxiangtu.top

Ruby: arr.uniq
来源：http://gwh.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://yss.yvedp.cn

[D16] 求和与平均值
来源：http://cgd.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ifz.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ldl.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmu.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ufx.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zjb.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://iqy.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qom.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://sxh.fengsongda.top

[D17] 最大值与最小值
来源：http://ohy.yj202588.top

Py:   max(arr);  min(arr)
来源：http://don.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://ufw.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mct.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://kai.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rip.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dcx.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://azo.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://png.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://hlo.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zay.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://yho.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bzp.jinqigfzy.top

TS:   nested.flat();
来源：http://lhi.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wnd.hcnkem.com

Go:   // 手写双层循环
来源：http://xfp.vqdsnc.cn

Ruby: nested.flatten
来源：http://qmr.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jbx.xinyue.icu

[D19] 按字段分组
来源：http://xjh.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bvs.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uvj.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pvz.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyh.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ubs.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://tjn.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uez.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sfh.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://kju.gotoacloud.top

Py:   Counter(arr)
来源：http://pyf.52xcode.cn

PHP:  array_count_values($arr);
来源：http://sux.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gbz.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jfa.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ntj.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://oyq.zdqjudy.top

Ruby: arr.tally
来源：http://ztq.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kzg.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://yxk.yonumen.top

Py:   x in arr
来源：http://ope.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://wgt.meibo888.top

JS:   arr.includes(x)
来源：http://wwr.sweek.top

TS:   arr.includes(x)
来源：http://abh.sysykeji.top

Java: list.contains(x)
来源：http://ldd.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://ylm.fzhhl.top

Ruby: arr.include?(x)
来源：http://yzp.svipenyu.cn

C#:   list.Contains(x)
来源：http://ouq.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://czp.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://duu.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dbv.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rto.bbcook.cn

TS:   [...arr];
来源：http://vfo.birdmap.top

Java: new ArrayList<>(list);
来源：http://naa.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zac.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://wst.svipenyu.cn

C#:   new List<int>(list);
来源：http://ujf.mhx1999.top

[D23] reduce 累积计算
来源：http://cjt.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nnp.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://biw.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pbc.yonumen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsg.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://las.fzhhl.top

Go:   // 手写循环
来源：http://obs.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rum.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sax.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://uvv.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wem.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kfy.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jqe.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qyz.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iny.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qxl.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vur.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nrg.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://lrb.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ydq.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kku.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://reg.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rss.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ibr.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ivg.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fuz.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nxx.aizwys.cn

[D26] 数组转字符串
来源：http://xov.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://nyf.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://clb.uphjek.com

JS:   arr.join(", ")
来源：http://byy.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://fus.gzhubu.top

Java: String.join(", ", list)
来源：http://hdj.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://zys.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://kan.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://utj.aizwys.cn

================================================================================
来源：http://eib.fktsv.cn

E. 字符串处理
来源：http://bbk.chenzaomai.com

================================================================================
来源：http://oyh.havefunace.top

[E01] 拼接字符串
来源：http://wmz.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://foi.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lvz.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://odl.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qjy.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hrv.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://llv.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://doa.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fks.vqdsnc.cn

[E02] 重复字符串
来源：http://nmk.xinyue.icu

Py:   "ab" * 3
来源：http://nyy.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://lse.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://gzr.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://zhv.andypj.xyz

Java: "ab".repeat(3)
来源：http://ppp.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://qeu.hcnkem.com

Ruby: "ab" * 3
来源：http://wap.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wrf.sweek.top

[E03] 截取子串
来源：http://orx.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgy.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjp.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ntp.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://fxz.xziqi.cn

Java: s.substring(1, 4)
来源：http://hpa.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cck.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qqz.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://aim.jqgufenzy.top

[E04] 查找子串位置
来源：http://wxg.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://ssv.fktsv.cn

PHP:  strpos($s, "x");
来源：http://vbi.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qbm.haohaochexian.top

TS:   s.indexOf("x")
来源：http://jvi.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://cid.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://agd.cqqwz.cn

Ruby: s.index("x")
来源：http://xma.jianghu66.top

C#:   s.IndexOf("x")
来源：http://vfq.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://bwv.hnqzz.top


<!-- 参考信息 -->