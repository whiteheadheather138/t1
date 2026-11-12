代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iwo.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://zpw.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bno.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://oyr.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dwz.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xpo.yj20258.top

Java: // 无解构
来源：http://dww.gogol.net.cn

Go:   // 无解构
来源：http://xui.shzxlz.cn

Ruby: a, b = pair
来源：http://iis.yueranfly.top

C#:   var (a, b) = pair;
来源：http://ocx.ydzc1.top

[C16] 函数 / 方法重载
来源：http://gta.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tqz.hfpthk.cn

PHP:  // 无重载
来源：http://bew.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gry.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://svi.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://doc.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://ixk.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://sdq.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lvb.kuanghao11.cn

================================================================================
来源：http://aux.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://cim.gogol.net.cn

================================================================================
来源：http://veg.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://uzj.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cjx.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hxj.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hwr.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdq.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fte.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://roo.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://sbk.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wra.shzxlz.cn

[D02] 追加元素到末尾
来源：http://rgl.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vyo.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oto.chenlongwang.top

JS:   arr.push(4);
来源：http://gzc.316326.xyz

TS:   arr.push(4);
来源：http://eik.ydjk.org.cn

Java: list.add(4);
来源：http://gta.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://llb.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://bfe.jlsjyb.cn

C#:   list.Add(4);
来源：http://ace.yj202588.top

[D03] 在指定位置插入元素
来源：http://syz.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://fla.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ozz.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qns.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://khm.bbcook.cn

Java: list.add(0, 0);
来源：http://ado.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://zle.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://esw.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://kjr.uphjek.com

[D04] 删除元素
来源：http://ief.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rmb.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yah.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tjf.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://ufq.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wgk.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jau.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gta.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rbv.hfpthk.cn

[D05] 访问与修改元素
来源：http://nab.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xpg.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfa.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://grq.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://ulm.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://cpl.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://vyi.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vbm.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yjz.chenlongwang.top

[D06] 数组长度
来源：http://vjp.dashuyun.cn

Py:   len(arr)
来源：http://lvc.hcnkem.com

PHP:  count($arr);
来源：http://glf.ivvv.top

JS:   arr.length
来源：http://fxm.ydzc1.top

TS:   arr.length
来源：http://sha.xylfe.cn

Java: list.size();
来源：http://tnj.xuetiantiany.cn

Go:   len(arr)
来源：http://szs.tian-w.cn

Ruby: arr.length; arr.size
来源：http://ehq.chenlongwang.top

C#:   list.Count;
来源：http://wlr.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://nww.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://brd.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://qqp.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://yhy.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://mju.yuxming.cn

Java: list.subList(1, 4);
来源：http://cuc.hcnkem.com

Go:   arr[1:4]
来源：http://ukj.vehdjk.com

Ruby: arr[1, 3]
来源：http://rur.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://lwc.sjlbkw.cn

[D08] 合并两个数组
来源：http://wvf.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://qng.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://uqm.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kqw.redwolf501.top

TS:   [...a, ...b];
来源：http://lpw.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://myh.ivvv.top

Go:   append(a, b...)
来源：http://kti.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://izd.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://rfh.fengsongda.top

[D09] 排序（升序）
来源：http://woa.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://vni.jqgufenzy.top

PHP:  sort($arr);
来源：http://tij.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://txh.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vcx.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mms.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vro.pycfn.com

Ruby: arr.sort
来源：http://xde.fengsongda.top

C#:   list.Sort();
来源：http://gor.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zsa.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://olb.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jxy.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wxh.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpz.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sqx.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opd.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xct.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vjy.tarul.cn

[D11] 反转数组
来源：http://pds.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://ccp.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://fyz.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://snb.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://fcf.xinyue.icu

Java: Collections.reverse(list);
来源：http://qcr.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://bpj.hcnkem.com

Ruby: arr.reverse
来源：http://sfp.zhengqikj.top

C#:   list.Reverse();
来源：http://xlr.yfazqb.com

[D12] 查找元素下标
来源：http://ols.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://ble.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aif.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rca.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wtd.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://geu.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://avy.yongpay.top

Ruby: arr.index(x)
来源：http://odm.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://hjn.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://ulk.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ntk.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wir.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://aet.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://puz.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qhg.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lpy.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dtn.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kly.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://gbi.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uvj.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bvl.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://oax.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://qpx.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fpy.zhixingplan.top

Go:   // 手写循环
来源：http://uvg.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://oos.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://buv.hcnkem.com

[D15] 去重
来源：http://erq.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jon.guannengcc.top

PHP:  array_unique($arr);
来源：http://zhy.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://uzf.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://yoj.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://khw.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wvd.zhengqikj.top

Ruby: arr.uniq
来源：http://udq.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://nlm.guannengcc.top

[D16] 求和与平均值
来源：http://gue.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sny.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xhx.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ysl.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgz.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eyb.yfazqb.com

Go:   // 手写循环累加
来源：http://ckl.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cdt.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://yfp.xuanzx.com

[D17] 最大值与最小值
来源：http://dku.uphjek.com

Py:   max(arr);  min(arr)
来源：http://jht.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://kcq.shuidangran.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zpf.cdnleiting.top

TS:   Math.max(...arr);
来源：http://ngt.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rhu.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vvs.316326.xyz

Ruby: arr.max;  arr.min
来源：http://uzt.316326.xyz

C#:   list.Max();  list.Min()
来源：http://uel.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://isi.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zev.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://vjq.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gsq.guannengcc.top

TS:   nested.flat();
来源：http://ndx.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jis.vehdjk.com

Go:   // 手写双层循环
来源：http://srj.zhiwuduotai.top

Ruby: nested.flatten
来源：http://fob.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ujd.yfazqb.com

[D19] 按字段分组
来源：http://rfz.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jga.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tmt.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pcf.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kiu.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgi.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://rgs.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ncf.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mrl.yj20258.top

[D20] 统计每个元素出现次数
来源：http://ezr.c1oappe.top

Py:   Counter(arr)
来源：http://kuj.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://llm.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eby.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqk.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ecw.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://ulb.tianlin.xyz

Ruby: arr.tally
来源：http://goc.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gma.redwolf501.top

[D21] 判断是否包含某元素
来源：http://esc.ywan-chungtsiang.top

Py:   x in arr
来源：http://mhr.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://vdt.jyoumei.cn

JS:   arr.includes(x)
来源：http://wmf.tian-w.cn

TS:   arr.includes(x)
来源：http://tia.yongpay.top

Java: list.contains(x)
来源：http://nzx.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://grd.cashguo.top

Ruby: arr.include?(x)
来源：http://yiu.xinyue.icu

C#:   list.Contains(x)
来源：http://shy.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://xri.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbj.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lbf.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oev.yanxiufei.cn

TS:   [...arr];
来源：http://hox.tian-w.cn

Java: new ArrayList<>(list);
来源：http://cbu.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://dbk.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://see.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://jhk.andypj.xyz

[D23] reduce 累积计算
来源：http://svc.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lec.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dal.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikf.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxj.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wxr.tian-w.cn

Go:   // 手写循环
来源：http://mqr.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kfr.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dzk.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://ysa.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dyy.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://roo.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tuk.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zup.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://llo.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://msy.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qvx.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qwq.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://khe.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ors.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ooi.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjz.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://brz.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://isy.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eot.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyr.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwq.fengsongda.top

[D26] 数组转字符串
来源：http://teh.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://fme.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://dqq.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://obv.tianlin.xyz

TS:   arr.join(", ")
来源：http://gbc.cashguo.top

Java: String.join(", ", list)
来源：http://mbj.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://era.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://kxx.cucudq.cn

C#:   string.Join(", ", list)
来源：http://bxm.havefunace.top

================================================================================
来源：http://whx.daxiang520.top

E. 字符串处理
来源：http://dnl.yuanzhike.top

================================================================================
来源：http://giu.yj202588.top

[E01] 拼接字符串
来源：http://otz.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ccm.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dzb.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ura.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xwt.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jtu.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mns.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://skf.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qka.jlsjyb.cn

[E02] 重复字符串
来源：http://mvw.gaohongyu789.top

Py:   "ab" * 3
来源：http://stz.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://fgn.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://qoi.zhengqikj.top

TS:   "ab".repeat(3)
来源：http://lxd.hesvh.cn

Java: "ab".repeat(3)
来源：http://exw.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://vra.hysaishi.cn

Ruby: "ab" * 3
来源：http://sjp.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nsm.ivvv.top

[E03] 截取子串
来源：http://pwq.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mbp.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxm.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wca.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://fmi.mhx1999.top

Java: s.substring(1, 4)
来源：http://bdb.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bmn.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zdh.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://lbp.xuanzx.com

[E04] 查找子串位置
来源：http://lkp.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://tfh.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://iyb.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jev.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://qis.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://nqa.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://nga.zhijiandao.cn

Ruby: s.index("x")
来源：http://udt.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://ftx.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xel.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fzv.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lip.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jmd.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vos.fanxiaobao.xyz


<!-- 参考信息 -->