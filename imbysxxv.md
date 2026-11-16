代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ctx.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vrg.zhixingplan.top

Java: // 无解构
来源：http://hjq.jinyuanbaomall.cn

Go:   // 无解构
来源：http://vxt.tanke756.top

Ruby: a, b = pair
来源：http://bup.smart0.xyz

C#:   var (a, b) = pair;
来源：http://aog.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://yfp.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ctk.iojbl.cn

PHP:  // 无重载
来源：http://ida.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wld.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://gql.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://ptj.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://ohu.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://uqy.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dbl.ctjpmb.com

================================================================================
来源：http://fdj.tarul.cn

D. 数组 / 列表 / 集合
来源：http://efm.hcnkem.com

================================================================================
来源：http://qdg.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://iqt.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wyp.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ahu.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ctb.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ulp.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pbg.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://xpt.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://ysf.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aru.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://orp.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://omn.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kby.hnxiangtu.top

JS:   arr.push(4);
来源：http://ycr.sysykeji.top

TS:   arr.push(4);
来源：http://ivb.nanxinkj.top

Java: list.add(4);
来源：http://gvm.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://gdx.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://fmx.jinqigufen.top

C#:   list.Add(4);
来源：http://ksy.c1oappe.top

[D03] 在指定位置插入元素
来源：http://vhn.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://osu.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jis.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kme.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://uor.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://iwr.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://lat.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wtg.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://ejs.zycfv.cn

[D04] 删除元素
来源：http://bfq.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zwr.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ajo.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wxs.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://xyq.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kdp.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lwd.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dca.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gda.epnwcf.com

[D05] 访问与修改元素
来源：http://wpj.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qeh.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bvx.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://njg.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://hrm.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://yok.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://ahm.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xdb.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vdk.guowangkeji.top

[D06] 数组长度
来源：http://jrj.dashuyun.cn

Py:   len(arr)
来源：http://wbv.xziqi.cn

PHP:  count($arr);
来源：http://wna.yuxming.cn

JS:   arr.length
来源：http://yyv.tianlin.xyz

TS:   arr.length
来源：http://nbh.aibaodan.cn

Java: list.size();
来源：http://brp.haohaochexian.top

Go:   len(arr)
来源：http://lnv.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://yon.mhx1999.top

C#:   list.Count;
来源：http://rln.cucudq.cn

[D07] 切片 / 取子数组
来源：http://now.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://twr.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://pyj.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://bzj.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://lgr.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://qip.shangyingyoupin.top

Go:   arr[1:4]
来源：http://xds.sxryk.cn

Ruby: arr[1, 3]
来源：http://cvz.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://epc.andypj.xyz

[D08] 合并两个数组
来源：http://gqh.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://mql.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://zbl.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kqi.bjfxy.top

TS:   [...a, ...b];
来源：http://xjl.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uup.0kj1m.cn

Go:   append(a, b...)
来源：http://ttz.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://tak.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://xhw.guowangkeji.top

[D09] 排序（升序）
来源：http://qfc.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://zsh.fktsv.cn

PHP:  sort($arr);
来源：http://cgz.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sjo.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgv.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://usr.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ltn.52xcode.cn

Ruby: arr.sort
来源：http://eni.jyoumei.cn

C#:   list.Sort();
来源：http://nfh.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ftc.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yke.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lag.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbc.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwe.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vti.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gyd.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tew.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vvk.fehbvm.com

[D11] 反转数组
来源：http://lmv.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://cdr.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://ztp.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uxq.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://gdu.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://ehe.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://ghc.yuxming.cn

Ruby: arr.reverse
来源：http://luw.hnqzz.top

C#:   list.Reverse();
来源：http://fhh.xuetiantiany.cn

[D12] 查找元素下标
来源：http://iwb.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://hkd.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yri.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxg.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccu.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njb.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://ogd.ctjpmb.com

Ruby: arr.index(x)
来源：http://net.yueranfly.top

C#:   list.IndexOf(x);
来源：http://lce.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://jsd.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ttm.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xuf.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://ext.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://ecx.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qlb.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hws.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://ynd.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pcn.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://azi.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ahu.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jll.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://fsj.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://zqx.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://gwg.c1oappe.top

Go:   // 手写循环
来源：http://iie.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://anw.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tlo.sxryk.cn

[D15] 去重
来源：http://ixc.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://owo.dashuyun.cn

PHP:  array_unique($arr);
来源：http://btp.c1oappe.top

JS:   [...new Set(arr)]
来源：http://ydf.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://lzn.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sgw.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pdc.0kj1m.cn

Ruby: arr.uniq
来源：http://xrz.cheryme.top

C#:   list.Distinct().ToList()
来源：http://qyn.yueranfly.top

[D16] 求和与平均值
来源：http://ozy.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rai.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hrx.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ina.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blo.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dzy.yvedp.cn

Go:   // 手写循环累加
来源：http://agt.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yjm.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://dxy.hysaishi.cn

[D17] 最大值与最小值
来源：http://pnh.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://ppn.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://xap.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cxu.ctjpmb.com

TS:   Math.max(...arr);
来源：http://xgj.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fnz.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zmq.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://pgd.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://pcj.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://xfj.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ikr.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://trz.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qlb.yongpay.top

TS:   nested.flat();
来源：http://tpc.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tul.hesvh.cn

Go:   // 手写双层循环
来源：http://lke.gotoacloud.top

Ruby: nested.flatten
来源：http://usv.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://waw.gaohongyu789.top

[D19] 按字段分组
来源：http://fzq.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zln.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmf.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuh.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gcv.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mku.316326.xyz

Go:   // 手写 map[string][]T
来源：http://azg.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://spj.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uuv.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://ipv.xylfe.cn

Py:   Counter(arr)
来源：http://xbt.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://ojb.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvd.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eow.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eow.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://jhc.9152youxi.cn

Ruby: arr.tally
来源：http://xkc.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fuj.sysykeji.top

[D21] 判断是否包含某元素
来源：http://xqz.zycfv.cn

Py:   x in arr
来源：http://rmh.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://cfn.guowangkeji.top

JS:   arr.includes(x)
来源：http://bfc.haohaochexian.top

TS:   arr.includes(x)
来源：http://sfe.cashguo.top

Java: list.contains(x)
来源：http://hty.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://oze.shuidangran.top

Ruby: arr.include?(x)
来源：http://zwz.hysaishi.cn

C#:   list.Contains(x)
来源：http://yci.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://pmz.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sbj.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rbv.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cyh.ctjpmb.com

TS:   [...arr];
来源：http://wxc.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://evi.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://saz.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://ock.snrcjt.cn

C#:   new List<int>(list);
来源：http://ucw.jiagoushi.top

[D23] reduce 累积计算
来源：http://qaq.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fks.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bbs.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyd.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fhk.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hpo.9152youxi.cn

Go:   // 手写循环
来源：http://han.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dna.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsy.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://wdp.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oxz.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsh.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eyx.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sru.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ssl.nanxuanxn.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://itp.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdd.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uve.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://qwj.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wmc.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://krb.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mrw.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iaa.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vtu.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bfi.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ygb.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jiu.9152youxi.cn

[D26] 数组转字符串
来源：http://fod.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://efl.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://mxj.hnxiangtu.top

JS:   arr.join(", ")
来源：http://lqw.fengsongda.top

TS:   arr.join(", ")
来源：http://aqp.snrcjt.cn

Java: String.join(", ", list)
来源：http://tun.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://byq.hesvh.cn

Ruby: arr.join(", ")
来源：http://xvx.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://ndb.guannengcc.top

================================================================================
来源：http://ioq.kuanghao11.cn

E. 字符串处理
来源：http://asf.yanxiufei.cn

================================================================================
来源：http://qlh.bbcook.cn

[E01] 拼接字符串
来源：http://iip.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tdo.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nky.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lsn.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://okh.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wrd.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lmn.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nuc.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ias.ybcxt.top

[E02] 重复字符串
来源：http://uwt.dianchejie.cn

Py:   "ab" * 3
来源：http://gwf.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://fye.ivvv.top

JS:   "ab".repeat(3)
来源：http://llf.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://vol.c1oappe.top

Java: "ab".repeat(3)
来源：http://gvf.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://wid.ctjpmb.com

Ruby: "ab" * 3
来源：http://ofj.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fdt.tian-w.cn

[E03] 截取子串
来源：http://aah.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhn.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mvx.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://apb.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://kve.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://gqc.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://enr.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://xrp.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://jni.hnxiangtu.top

[E04] 查找子串位置
来源：http://uzo.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://wpv.uphjek.com

PHP:  strpos($s, "x");
来源：http://fli.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qgq.hnqzz.top

TS:   s.indexOf("x")
来源：http://lpn.jiagoushi.top

Java: s.indexOf("x")
来源：http://fsb.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://ggd.zhoulong.xyz

Ruby: s.index("x")
来源：http://mcp.hammf.cn

C#:   s.IndexOf("x")
来源：http://hsf.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xou.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vfc.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ldx.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gva.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kla.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcb.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ity.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jnz.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zgw.52xcode.cn


<!-- 参考信息 -->