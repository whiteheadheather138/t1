代发 wailian999

Ruby: a, b = pair
来源：http://pzy.fehbvm.com

C#:   var (a, b) = pair;
来源：http://eqv.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://drr.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://our.haohaochexian.top

PHP:  // 无重载
来源：http://krf.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iqp.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://nto.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://pqn.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://cis.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://ehc.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mkw.sweek.top

================================================================================
来源：http://ufe.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://cyh.316326.xyz

================================================================================
来源：http://xkb.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://tgs.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pfd.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iry.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fzt.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hsn.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ihb.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://ksk.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://pcx.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jfn.gogol.net.cn

[D02] 追加元素到末尾
来源：http://gtt.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nza.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hzt.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://heu.hnqzz.top

TS:   arr.push(4);
来源：http://kss.pycfn.com

Java: list.add(4);
来源：http://ptp.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://xkp.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ebr.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://mbt.shuidangran.top

[D03] 在指定位置插入元素
来源：http://zur.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://pkz.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bqp.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://brt.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://xua.bbcook.cn

Java: list.add(0, 0);
来源：http://xqz.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://dar.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://omr.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://eqn.52xcode.cn

[D04] 删除元素
来源：http://ccw.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://odh.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twx.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fjc.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://goi.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vey.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sau.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czq.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ztf.aibaodan.cn

[D05] 访问与修改元素
来源：http://gho.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ztm.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iuq.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vvq.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://fxw.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://lbs.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://tzl.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://thr.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lon.havefunace.top

[D06] 数组长度
来源：http://gyh.yj20258.top

Py:   len(arr)
来源：http://amb.xuanzx.com

PHP:  count($arr);
来源：http://vqc.gotoacloud.top

JS:   arr.length
来源：http://tqx.yj202588.top

TS:   arr.length
来源：http://fed.xuanzx.com

Java: list.size();
来源：http://dwn.sjlbkw.cn

Go:   len(arr)
来源：http://gpe.bbcook.cn

Ruby: arr.length; arr.size
来源：http://sqm.jinyuanbaomall.cn

C#:   list.Count;
来源：http://ezp.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://hxj.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nzj.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cfg.yj20258.top

JS:   arr.slice(1, 4);
来源：http://xyx.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://ozd.tian-w.cn

Java: list.subList(1, 4);
来源：http://nyo.meibo888.top

Go:   arr[1:4]
来源：http://qvj.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://lee.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://ebk.c1oappe.top

[D08] 合并两个数组
来源：http://izi.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://mck.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://ixn.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wix.zdbjq.cn

TS:   [...a, ...b];
来源：http://aps.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bbc.xziqi.cn

Go:   append(a, b...)
来源：http://lsj.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://hnc.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://unv.shzxlz.cn

[D09] 排序（升序）
来源：http://uaz.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://wyk.jinqigufen.top

PHP:  sort($arr);
来源：http://eak.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qyt.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vky.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ekc.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ozs.hfpthk.cn

Ruby: arr.sort
来源：http://nbh.gzhubu.top

C#:   list.Sort();
来源：http://sbu.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rrb.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://opa.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://boi.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxq.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfz.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://laq.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mah.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dxs.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wdo.epnwcf.com

[D11] 反转数组
来源：http://mde.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://ldt.nwbrower.top

PHP:  array_reverse($arr);
来源：http://sdm.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xdm.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://chi.tanke756.top

Java: Collections.reverse(list);
来源：http://oxd.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://tuj.xuanzx.com

Ruby: arr.reverse
来源：http://cur.vqdsnc.cn

C#:   list.Reverse();
来源：http://dmx.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://lcm.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://yih.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ayd.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yyw.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mqd.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lvo.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://lth.yj20258888.top

Ruby: arr.index(x)
来源：http://hcp.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://ilj.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://wky.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://awx.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzu.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://pnt.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://rpy.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jrh.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xqr.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://ucm.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nju.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://yiq.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mbk.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vvv.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://ziu.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://boz.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hjo.fktsv.cn

Go:   // 手写循环
来源：http://tnr.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://ofz.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://krj.zycfv.cn

[D15] 去重
来源：http://kdt.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vhn.gotoacloud.top

PHP:  array_unique($arr);
来源：http://jtm.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://amy.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://ifw.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mxp.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://waz.feifeiyinyue.top

Ruby: arr.uniq
来源：http://ayb.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://pii.vehdjk.com

[D16] 求和与平均值
来源：http://dud.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://piu.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vgo.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tng.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vua.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ttf.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://shx.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdu.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://wua.c1oappe.top

[D17] 最大值与最小值
来源：http://pjx.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://vcl.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://ist.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mye.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://bah.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://say.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pwg.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://uls.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://dfd.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://bcc.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bau.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://irr.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qzc.aibaodan.cn

TS:   nested.flat();
来源：http://ibc.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ixw.gaohongyu789.top

Go:   // 手写双层循环
来源：http://hai.gogol.net.cn

Ruby: nested.flatten
来源：http://xks.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pkx.yangfankeji.com

[D19] 按字段分组
来源：http://qrw.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jej.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xlm.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jyv.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lpf.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xvj.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://rxm.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cmm.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nhx.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://ohs.zhengqikj.top

Py:   Counter(arr)
来源：http://nfr.smart0.xyz

PHP:  array_count_values($arr);
来源：http://rht.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpc.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://izq.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ncp.sxryk.cn

Go:   // 手写 map[T]int
来源：http://ieu.epnwcf.com

Ruby: arr.tally
来源：http://aiv.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bfn.daxiang520.top

[D21] 判断是否包含某元素
来源：http://omh.bbcook.cn

Py:   x in arr
来源：http://smc.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://rzi.gogol.net.cn

JS:   arr.includes(x)
来源：http://iif.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://lgr.gzhubu.top

Java: list.contains(x)
来源：http://rld.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://mxh.cashguo.top

Ruby: arr.include?(x)
来源：http://tds.ybcxt.top

C#:   list.Contains(x)
来源：http://ezq.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://rvh.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpa.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jww.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://orb.zdbjq.cn

TS:   [...arr];
来源：http://gwj.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://tqa.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://owx.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://gpu.xinyue.icu

C#:   new List<int>(list);
来源：http://xsj.jlsjyb.cn

[D23] reduce 累积计算
来源：http://hci.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nah.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bng.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffh.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ygo.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://owq.yuanzhike.top

Go:   // 手写循环
来源：http://dnx.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdy.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yfh.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://kub.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qjr.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ktd.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iws.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fgj.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uzu.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ufv.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qpq.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cmk.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://xxz.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fus.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tbu.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uqg.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lsr.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yqu.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://exs.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mkt.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bfy.chenzaomai.com

[D26] 数组转字符串
来源：http://vmf.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://fgk.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://mfm.svipenyu.cn

JS:   arr.join(", ")
来源：http://myw.kuanghao11.cn

TS:   arr.join(", ")
来源：http://cfv.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://rbl.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://oja.tarul.cn

Ruby: arr.join(", ")
来源：http://ydt.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://peh.sufxvd.cn

================================================================================
来源：http://okk.guowangkeji.top

E. 字符串处理
来源：http://jgx.zhoulong.xyz

================================================================================
来源：http://cug.ybcxt.top

[E01] 拼接字符串
来源：http://wwd.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://utb.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://apx.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kre.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oao.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://avs.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tkm.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uhn.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xdd.zhengqikj.top

[E02] 重复字符串
来源：http://com.gogol.net.cn

Py:   "ab" * 3
来源：http://vno.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://hus.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://mdo.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://mki.dashuyun.cn

Java: "ab".repeat(3)
来源：http://wgw.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://ydh.tarul.cn

Ruby: "ab" * 3
来源：http://zft.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zjd.cdnleiting.top

[E03] 截取子串
来源：http://jxu.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ftb.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://etr.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xho.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://kol.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://egv.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nqc.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://vpo.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://pjy.cqqwz.cn

[E04] 查找子串位置
来源：http://shd.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://dmj.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://qju.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://efu.hammf.cn

TS:   s.indexOf("x")
来源：http://tda.hysaishi.cn

Java: s.indexOf("x")
来源：http://rds.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://dzw.vqdsnc.cn

Ruby: s.index("x")
来源：http://hoi.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://evd.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://izk.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kzw.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://txd.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpe.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cfu.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uik.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gyb.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sqh.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kjd.hfpthk.cn

[E06] 替换子串
来源：http://rih.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ijf.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://ebt.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eds.xylfe.cn


<!-- 参考信息 -->