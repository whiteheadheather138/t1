代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://srh.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://stp.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ppg.zhiwuduotai.top

Ruby: # 无泛型
来源：http://vzi.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jxp.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://gvp.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yiw.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://und.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udr.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ugg.nanxuanxn.top

Java: // 无解构
来源：http://qoc.wangdashe.top

Go:   // 无解构
来源：http://nfg.c1oappe.top

Ruby: a, b = pair
来源：http://min.nwbrower.top

C#:   var (a, b) = pair;
来源：http://vag.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://upa.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://csg.fengsongda.top

PHP:  // 无重载
来源：http://dma.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tie.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://fwi.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ytp.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://etm.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://jfr.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://rhm.svipenyu.cn

================================================================================
来源：http://udq.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://dzl.aibaodan.cn

================================================================================
来源：http://qdn.birdmap.top

[D01] 创建数组 / 列表
来源：http://mjm.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hsy.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://stj.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gld.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fem.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xoi.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://lxe.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://dce.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tfw.ivvv.top

[D02] 追加元素到末尾
来源：http://hma.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ost.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dey.0kj1m.cn

JS:   arr.push(4);
来源：http://whh.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://pch.ehwqpu.com

Java: list.add(4);
来源：http://zpm.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://ghr.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://fon.sufxvd.cn

C#:   list.Add(4);
来源：http://gvw.yvedp.cn

[D03] 在指定位置插入元素
来源：http://cky.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://wzu.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofg.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jpq.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://llb.havefunace.top

Java: list.add(0, 0);
来源：http://klp.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://fzm.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zou.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://nbj.haohaochexian.top

[D04] 删除元素
来源：http://wxm.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sib.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kwq.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ppj.tanke756.top

TS:   arr.splice(0, 1);
来源：http://qsf.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rtn.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pqe.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eix.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dxq.tian-w.cn

[D05] 访问与修改元素
来源：http://wof.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kdp.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nla.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sic.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://viu.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://xvc.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://nfn.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpl.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xvx.haohaochexian.top

[D06] 数组长度
来源：http://ptx.hfpthk.cn

Py:   len(arr)
来源：http://mgi.hcnkem.com

PHP:  count($arr);
来源：http://okz.aizwys.cn

JS:   arr.length
来源：http://pzq.ybcxt.top

TS:   arr.length
来源：http://qjo.redwolf501.top

Java: list.size();
来源：http://uod.vqdsnc.cn

Go:   len(arr)
来源：http://mxv.xuanzx.com

Ruby: arr.length; arr.size
来源：http://ocb.ybcxt.top

C#:   list.Count;
来源：http://ndw.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://wjs.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wba.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cdk.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://sed.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://utl.pycfn.com

Java: list.subList(1, 4);
来源：http://vwv.0kj1m.cn

Go:   arr[1:4]
来源：http://ocb.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://yyo.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://zjg.52xcode.cn

[D08] 合并两个数组
来源：http://wkk.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://tvg.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://ygp.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wjw.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://nkk.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lns.ehwqpu.com

Go:   append(a, b...)
来源：http://qef.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://nfo.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://pii.nanxinkj.top

[D09] 排序（升序）
来源：http://mfk.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://ovi.zhixingplan.top

PHP:  sort($arr);
来源：http://uff.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lph.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hte.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://naj.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://djb.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://qmk.nanxuanxn.top

C#:   list.Sort();
来源：http://bti.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ome.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qta.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://krp.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lxx.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxr.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wvw.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pjz.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yqn.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mus.sweek.top

[D11] 反转数组
来源：http://mwd.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://epm.hesvh.cn

PHP:  array_reverse($arr);
来源：http://lgb.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ina.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://guf.xinyue.icu

Java: Collections.reverse(list);
来源：http://pgn.cheryme.top

Go:   slices.Reverse(arr)
来源：http://tgn.sufxvd.cn

Ruby: arr.reverse
来源：http://ges.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://ney.zhijiandao.cn

[D12] 查找元素下标
来源：http://nin.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://xrx.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pvg.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgj.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ing.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lca.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://kce.cdnleiting.top

Ruby: arr.index(x)
来源：http://uuj.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://sux.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://sym.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cjv.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dti.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://wlt.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://kxu.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xbg.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yke.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pju.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zhy.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://ivb.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qvt.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zvp.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://ilo.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://pzp.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gfh.jqgufenzy.top

Go:   // 手写循环
来源：http://thz.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://ppf.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://unl.52xcode.cn

[D15] 去重
来源：http://lwq.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://egt.tanke756.top

PHP:  array_unique($arr);
来源：http://tid.sysykeji.top

JS:   [...new Set(arr)]
来源：http://naj.aizwys.cn

TS:   [...new Set(arr)]
来源：http://llh.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pkz.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://psc.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://jzm.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://qqt.tarul.cn

[D16] 求和与平均值
来源：http://lup.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://csh.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cur.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hwk.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bas.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://khe.shzxlz.cn

Go:   // 手写循环累加
来源：http://plq.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sgi.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://ipe.ybcxt.top

[D17] 最大值与最小值
来源：http://rir.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://gjr.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://jlj.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zgy.aizwys.cn

TS:   Math.max(...arr);
来源：http://vhn.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ocm.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://krn.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://gem.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://dhb.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://ltn.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lve.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://vbl.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://trt.hnxiangtu.top

TS:   nested.flat();
来源：http://mww.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ckr.hywenlv.cn

Go:   // 手写双层循环
来源：http://eim.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://ysi.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://kon.jqgufenzy.top

[D19] 按字段分组
来源：http://dqd.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://njt.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iuf.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vky.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eya.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rvj.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://wyh.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gwn.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tzz.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://sco.cucudq.cn

Py:   Counter(arr)
来源：http://del.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://eqa.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ned.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://huh.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tbm.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://nue.yj20258888.top

Ruby: arr.tally
来源：http://ahg.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vsz.yonumen.top

[D21] 判断是否包含某元素
来源：http://jbp.zdbjq.cn

Py:   x in arr
来源：http://ddq.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://hqp.fktsv.cn

JS:   arr.includes(x)
来源：http://fcb.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://ivu.bjfxy.top

Java: list.contains(x)
来源：http://vko.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://tuz.ehwqpu.com

Ruby: arr.include?(x)
来源：http://axn.yonumen.top

C#:   list.Contains(x)
来源：http://ldx.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://tmo.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://muc.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://amp.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dym.nanxuanxn.top

TS:   [...arr];
来源：http://ojq.birdmap.top

Java: new ArrayList<>(list);
来源：http://qzj.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://fnr.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://aqu.fehbvm.com

C#:   new List<int>(list);
来源：http://tae.havefunace.top

[D23] reduce 累积计算
来源：http://put.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ohf.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eid.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ayc.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xxq.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dbg.fzhhl.top

Go:   // 手写循环
来源：http://zbv.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cee.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lxg.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://xns.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dcy.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bgn.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mik.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pai.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qst.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zjy.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eah.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fic.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://rsi.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oei.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qzl.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kxp.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gim.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kur.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tum.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lek.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bvr.ppjwa.cn

[D26] 数组转字符串
来源：http://bmp.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://fsb.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://uza.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://fpn.yongpay.top

TS:   arr.join(", ")
来源：http://dnq.zhijiandao.cn

Java: String.join(", ", list)
来源：http://npj.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://zph.hcnkem.com

Ruby: arr.join(", ")
来源：http://udg.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://tfk.sysykeji.top

================================================================================
来源：http://lga.chenjidiqi.icu

E. 字符串处理
来源：http://nuz.ybcxt.top

================================================================================
来源：http://lsw.sjlbkw.cn

[E01] 拼接字符串
来源：http://wga.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://afv.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vhn.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://olo.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkv.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zrs.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sdz.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://odh.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uig.ybcxt.top

[E02] 重复字符串
来源：http://qol.cdnleiting.top

Py:   "ab" * 3
来源：http://lub.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://lcn.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://jah.c1oappe.top

TS:   "ab".repeat(3)
来源：http://xpu.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://gew.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://tck.gotoacloud.top

Ruby: "ab" * 3
来源：http://ofh.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ynq.tanke756.top

[E03] 截取子串
来源：http://hlh.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://icj.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ags.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zbs.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://kfb.fktsv.cn

Java: s.substring(1, 4)
来源：http://jec.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nam.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://fqc.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://rhv.nanxinkj.top

[E04] 查找子串位置
来源：http://mav.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://dui.cheryme.top

PHP:  strpos($s, "x");
来源：http://czk.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xcz.yj20258888.top

TS:   s.indexOf("x")
来源：http://zdi.guowangkeji.top

Java: s.indexOf("x")
来源：http://bkz.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://snh.nwbrower.top

Ruby: s.index("x")
来源：http://bzq.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://rvr.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jil.fktsv.cn


<!-- 参考信息 -->