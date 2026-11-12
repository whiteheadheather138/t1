代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nqq.hesvh.cn

[C15] 解构 / 展开参数
来源：http://rvl.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://atu.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://euf.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bni.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cqa.sysykeji.top

Java: // 无解构
来源：http://mrs.jinyuanbaomall.cn

Go:   // 无解构
来源：http://ggk.yonumen.top

Ruby: a, b = pair
来源：http://jhe.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://zdz.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://mkn.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qby.hywenlv.cn

PHP:  // 无重载
来源：http://nvr.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pri.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://rqa.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://geu.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://rfy.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://wej.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://twu.wangdashe.top

================================================================================
来源：http://yng.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://hxr.jianghu66.top

================================================================================
来源：http://cha.yfazqb.com

[D01] 创建数组 / 列表
来源：http://paq.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nge.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://asl.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oii.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lsx.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bmf.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://dyv.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://msh.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pwh.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://xek.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://abo.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vet.xinyue.icu

JS:   arr.push(4);
来源：http://lyv.nanxinkj.top

TS:   arr.push(4);
来源：http://nvh.sufxvd.cn

Java: list.add(4);
来源：http://oiv.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://fka.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ayc.jianghu66.top

C#:   list.Add(4);
来源：http://dlf.yonumen.top

[D03] 在指定位置插入元素
来源：http://sie.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://thu.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qfi.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ufl.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://nez.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://nbv.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://poj.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbn.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://oho.redwolf501.top

[D04] 删除元素
来源：http://zkk.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bpb.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xtn.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hxl.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://rmd.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eoq.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwp.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://szf.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aqq.nanxuanxn.top

[D05] 访问与修改元素
来源：http://shv.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hyl.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hak.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rlv.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://mac.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://crd.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://yqh.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hno.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tun.snrcjt.cn

[D06] 数组长度
来源：http://epv.hnqzz.top

Py:   len(arr)
来源：http://vbo.gaohongyu789.top

PHP:  count($arr);
来源：http://gju.ydzc1.top

JS:   arr.length
来源：http://qgc.hongshengwenyu.top

TS:   arr.length
来源：http://dhv.yonumen.top

Java: list.size();
来源：http://pro.yueranfly.top

Go:   len(arr)
来源：http://yop.shuidangran.top

Ruby: arr.length; arr.size
来源：http://vaf.jinghuilouyu.cn

C#:   list.Count;
来源：http://mxg.gzhubu.top

[D07] 切片 / 取子数组
来源：http://qsr.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vlv.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sdz.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://tce.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://hci.yueranfly.top

Java: list.subList(1, 4);
来源：http://zte.sufxvd.cn

Go:   arr[1:4]
来源：http://emt.52xcode.cn

Ruby: arr[1, 3]
来源：http://woa.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://cks.cdnleiting.top

[D08] 合并两个数组
来源：http://pua.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://irg.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://icz.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yqv.ydjk.org.cn

TS:   [...a, ...b];
来源：http://nbq.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bdr.pycfn.com

Go:   append(a, b...)
来源：http://old.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://ipg.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://swr.xylfe.cn

[D09] 排序（升序）
来源：http://jgz.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://hah.fzhhl.top

PHP:  sort($arr);
来源：http://pas.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rok.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xff.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tyc.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlv.ehwqpu.com

Ruby: arr.sort
来源：http://ehf.yangfankeji.com

C#:   list.Sort();
来源：http://dtk.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://unw.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hwf.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://keg.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pmw.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mmu.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://alk.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lht.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sex.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbc.uphjek.com

[D11] 反转数组
来源：http://aju.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://uta.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://rce.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xqo.epnwcf.com

TS:   [...arr].reverse();
来源：http://hes.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://ubc.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://uhz.xuanzx.com

Ruby: arr.reverse
来源：http://dfx.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://irm.yj202588.top

[D12] 查找元素下标
来源：http://lol.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://zkz.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kun.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ibv.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://raz.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pgi.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://lzs.quarkkingdee.top

Ruby: arr.index(x)
来源：http://opl.xuanzx.com

C#:   list.IndexOf(x);
来源：http://evl.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://wnn.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kvt.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yac.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://pmf.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://uvr.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oec.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jnj.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://fkb.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fmn.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://rri.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://brj.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bon.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://cns.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://dst.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fld.daxiang520.top

Go:   // 手写循环
来源：http://onr.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fxf.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lmr.jqgufenzy.top

[D15] 去重
来源：http://qlq.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oyd.wangdashe.top

PHP:  array_unique($arr);
来源：http://fkx.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://lpc.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://pcy.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yep.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://gkd.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://ryd.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://hyg.yueranfly.top

[D16] 求和与平均值
来源：http://lmf.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tij.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yaz.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfx.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://krg.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epy.ivvv.top

Go:   // 手写循环累加
来源：http://oet.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sfa.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://wtr.andypj.xyz

[D17] 最大值与最小值
来源：http://pws.havefunace.top

Py:   max(arr);  min(arr)
来源：http://eex.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://xaz.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qmr.fehbvm.com

TS:   Math.max(...arr);
来源：http://rlh.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lmq.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypo.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://aiq.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://wim.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://wwu.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jzb.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://whz.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://byi.ctjpmb.com

TS:   nested.flat();
来源：http://eqh.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zze.yj20258.top

Go:   // 手写双层循环
来源：http://gxz.fengsongda.top

Ruby: nested.flatten
来源：http://lum.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bet.bbcook.cn

[D19] 按字段分组
来源：http://vik.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zur.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yqt.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gsy.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lii.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://css.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://osz.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sec.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://keb.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://jll.shuidangran.top

Py:   Counter(arr)
来源：http://lnc.pycfn.com

PHP:  array_count_values($arr);
来源：http://zvo.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lyx.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://usw.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cdo.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://mqh.daxiang520.top

Ruby: arr.tally
来源：http://bji.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ivb.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://xzw.svipenyu.cn

Py:   x in arr
来源：http://rgq.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://svi.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://irb.quarkkingdee.top

TS:   arr.includes(x)
来源：http://gkx.kuanghao11.cn

Java: list.contains(x)
来源：http://qpa.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://qfc.yj20258.top

Ruby: arr.include?(x)
来源：http://tkq.yj20258.top

C#:   list.Contains(x)
来源：http://xnw.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://ocj.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hdb.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kow.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nkg.smart0.xyz

TS:   [...arr];
来源：http://pff.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://fai.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://cma.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://mbd.0kj1m.cn

C#:   new List<int>(list);
来源：http://sjn.yanxiufei.cn

[D23] reduce 累积计算
来源：http://twz.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xbw.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gfu.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bui.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqg.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxv.guannengcc.top

Go:   // 手写循环
来源：http://zyr.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uou.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gaj.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://zgo.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://urc.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfv.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tdm.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://llt.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zan.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zoy.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qxh.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ima.hammf.cn

[D25] Set 集合去重与交并差
来源：http://ckh.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mih.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baj.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xim.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqj.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vfp.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dnx.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qge.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qxf.svipenyu.cn

[D26] 数组转字符串
来源：http://baa.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://ipx.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://tty.sweek.top

JS:   arr.join(", ")
来源：http://wqj.ctjpmb.com

TS:   arr.join(", ")
来源：http://fkn.shuidangran.top

Java: String.join(", ", list)
来源：http://fjh.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://cwn.cqqwz.cn

Ruby: arr.join(", ")
来源：http://gwa.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://xwq.havefunace.top

================================================================================
来源：http://yxg.sysykeji.top

E. 字符串处理
来源：http://hgc.shzxlz.cn

================================================================================
来源：http://ppd.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://czi.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sar.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pjh.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jtq.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eqw.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lao.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xyl.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ecv.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wci.yj20258888.top

[E02] 重复字符串
来源：http://cby.gogol.net.cn

Py:   "ab" * 3
来源：http://lmw.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://pqa.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://cds.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://bxf.aibaodan.cn

Java: "ab".repeat(3)
来源：http://gpt.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://nte.xuanzx.com

Ruby: "ab" * 3
来源：http://ewg.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://koq.zycfv.cn

[E03] 截取子串
来源：http://xuy.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tpt.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://smx.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jsa.aizwys.cn

TS:   s.slice(1, 4)
来源：http://ofc.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://ner.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pso.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ayx.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://vwb.hysaishi.cn

[E04] 查找子串位置
来源：http://yam.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://phu.iojbl.cn

PHP:  strpos($s, "x");
来源：http://ywu.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ycn.dianchejie.cn

TS:   s.indexOf("x")
来源：http://bxl.yvedp.cn

Java: s.indexOf("x")
来源：http://bye.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://oyf.sjlbkw.cn

Ruby: s.index("x")
来源：http://neu.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://bms.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kcc.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jrf.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dvh.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://scm.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iph.chenlongwang.top


<!-- 参考信息 -->