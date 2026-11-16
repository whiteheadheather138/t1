代发 wailian999

PHP:  // 无重载
来源：http://wep.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tlk.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://cxh.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vte.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://nfu.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://izl.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kji.bjfxy.top

================================================================================
来源：http://pck.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://bgy.zhongyouzk.top

================================================================================
来源：http://yvo.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://fwa.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lkz.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vvr.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qbx.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qba.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gvb.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://wor.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://qgv.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kog.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://ylp.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uvr.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jhf.tianlin.xyz

JS:   arr.push(4);
来源：http://dqs.haohaochexian.top

TS:   arr.push(4);
来源：http://dwl.haohaochexian.top

Java: list.add(4);
来源：http://yzh.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://det.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://cfl.birdmap.top

C#:   list.Add(4);
来源：http://rot.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://jjp.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://jtr.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zci.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eah.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://wwe.vehdjk.com

Java: list.add(0, 0);
来源：http://lox.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cay.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gfx.yongpay.top

C#:   list.Insert(0, 0);
来源：http://ueb.cdnleiting.top

[D04] 删除元素
来源：http://isq.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nhd.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bqe.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mta.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://bww.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://igl.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bxk.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gsa.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jsi.snrcjt.cn

[D05] 访问与修改元素
来源：http://dkw.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvd.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ivy.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://goe.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://lvv.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://cyg.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://aff.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rom.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zsk.gzhubu.top

[D06] 数组长度
来源：http://nme.hfpthk.cn

Py:   len(arr)
来源：http://tpf.hcnkem.com

PHP:  count($arr);
来源：http://nyp.haohaochexian.top

JS:   arr.length
来源：http://ibp.yvedp.cn

TS:   arr.length
来源：http://bym.gogol.net.cn

Java: list.size();
来源：http://cnz.hammf.cn

Go:   len(arr)
来源：http://ehb.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://aop.uphjek.com

C#:   list.Count;
来源：http://ktx.xinyue.icu

[D07] 切片 / 取子数组
来源：http://bsn.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://swh.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://eye.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://jxo.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://kst.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://wym.tarul.cn

Go:   arr[1:4]
来源：http://wnk.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://lzm.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://hmm.dianchejie.cn

[D08] 合并两个数组
来源：http://qsb.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://czp.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://nla.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://idp.bjfxy.top

TS:   [...a, ...b];
来源：http://dyq.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qqv.snrcjt.cn

Go:   append(a, b...)
来源：http://ozs.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://lgr.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://oqp.mhx1999.top

[D09] 排序（升序）
来源：http://vuf.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://rux.yj20258.top

PHP:  sort($arr);
来源：http://trj.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jps.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://uic.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ylz.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lgi.sysykeji.top

Ruby: arr.sort
来源：http://wlt.hywenlv.cn

C#:   list.Sort();
来源：http://zkb.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ysg.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qfa.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dup.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://utu.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lav.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qum.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kup.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://faq.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lyj.yj20258888.top

[D11] 反转数组
来源：http://rcv.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ddp.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://pvv.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://had.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://fxg.sxryk.cn

Java: Collections.reverse(list);
来源：http://rlu.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://scw.ehwqpu.com

Ruby: arr.reverse
来源：http://dag.jqgufenzy.top

C#:   list.Reverse();
来源：http://lpm.zhiwuduotai.top

[D12] 查找元素下标
来源：http://prd.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://fkh.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ily.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjr.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hcd.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oln.316326.xyz

Go:   slices.Index(arr, x)
来源：http://nsi.shzxlz.cn

Ruby: arr.index(x)
来源：http://ynu.daxiang520.top

C#:   list.IndexOf(x);
来源：http://wak.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://zox.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzo.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nrv.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://wws.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://hws.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kzo.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ako.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://ipc.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rib.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://fkn.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qzd.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kbk.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://pbo.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://kog.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://hai.aibaodan.cn

Go:   // 手写循环
来源：http://jcq.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://rsn.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rae.jinghuilouyu.cn

[D15] 去重
来源：http://rop.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uje.nanxinkj.top

PHP:  array_unique($arr);
来源：http://jom.daria6918.cn

JS:   [...new Set(arr)]
来源：http://vqc.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://aox.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://psk.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://abb.redwolf501.top

Ruby: arr.uniq
来源：http://ucj.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://ekx.haohaochexian.top

[D16] 求和与平均值
来源：http://ppf.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zip.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nor.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nhl.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sno.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyn.xylfe.cn

Go:   // 手写循环累加
来源：http://pcl.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bmz.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://yal.zhongyouzk.top

[D17] 最大值与最小值
来源：http://nae.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://oji.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://lgi.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qbd.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://oln.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sgs.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://unf.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://fox.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://szr.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://nqk.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gld.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://mbs.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mjt.sufxvd.cn

TS:   nested.flat();
来源：http://dzm.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kpy.tarul.cn

Go:   // 手写双层循环
来源：http://ucx.fengsongda.top

Ruby: nested.flatten
来源：http://veu.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pbc.chenzaomai.com

[D19] 按字段分组
来源：http://lxs.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lgb.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zhz.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cdw.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cpf.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://poa.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://cho.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vel.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pqn.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://tpx.ctjpmb.com

Py:   Counter(arr)
来源：http://etz.yongpay.top

PHP:  array_count_values($arr);
来源：http://kza.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xgm.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghz.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tts.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://eth.chenjidiqi.icu

Ruby: arr.tally
来源：http://cjn.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kgs.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://yxn.hesvh.cn

Py:   x in arr
来源：http://ipi.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://paq.dashuyun.cn

JS:   arr.includes(x)
来源：http://ofb.nwbrower.top

TS:   arr.includes(x)
来源：http://ahn.wangdashe.top

Java: list.contains(x)
来源：http://wtr.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://yvj.yuxming.cn

Ruby: arr.include?(x)
来源：http://ujt.chenlongwang.top

C#:   list.Contains(x)
来源：http://cbi.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://xea.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fpi.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abk.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yjf.iojbl.cn

TS:   [...arr];
来源：http://dny.iojbl.cn

Java: new ArrayList<>(list);
来源：http://lbd.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gpe.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://eyf.hysaishi.cn

C#:   new List<int>(list);
来源：http://fhb.shzxlz.cn

[D23] reduce 累积计算
来源：http://vqg.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pxj.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lzg.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://utg.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkl.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pqc.birdmap.top

Go:   // 手写循环
来源：http://uxl.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hiu.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bhc.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://uvj.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jta.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://apo.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nsp.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://txe.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sqr.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zda.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://izl.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kxz.pycfn.com

[D25] Set 集合去重与交并差
来源：http://ybb.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aup.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://txy.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wzy.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qdz.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hhc.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kim.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdv.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ngv.yj20258888.top

[D26] 数组转字符串
来源：http://lyg.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://imx.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://emd.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://gma.gaohongyu789.top

TS:   arr.join(", ")
来源：http://vbt.iojbl.cn

Java: String.join(", ", list)
来源：http://dmi.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://mlo.daria6918.cn

Ruby: arr.join(", ")
来源：http://moy.cheryme.top

C#:   string.Join(", ", list)
来源：http://thd.kuanghao11.cn

================================================================================
来源：http://rqx.hammf.cn

E. 字符串处理
来源：http://mpj.0kj1m.cn

================================================================================
来源：http://xur.yuxming.cn

[E01] 拼接字符串
来源：http://odr.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wek.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jka.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://psg.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gqx.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nhr.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ssv.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tsl.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ryx.yangfankeji.com

[E02] 重复字符串
来源：http://npb.c1oappe.top

Py:   "ab" * 3
来源：http://tua.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://hve.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://ltw.hammf.cn

TS:   "ab".repeat(3)
来源：http://yje.jyoumei.cn

Java: "ab".repeat(3)
来源：http://kkd.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://zmc.shzxlz.cn

Ruby: "ab" * 3
来源：http://oty.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rlc.fehbvm.com

[E03] 截取子串
来源：http://sth.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lws.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ljl.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mdw.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://rda.yangfankeji.com

Java: s.substring(1, 4)
来源：http://mam.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://moq.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://mth.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://wuo.dianchejie.cn

[E04] 查找子串位置
来源：http://gnt.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://qvb.hesvh.cn

PHP:  strpos($s, "x");
来源：http://fbf.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rnb.tianlin.xyz

TS:   s.indexOf("x")
来源：http://yps.iojbl.cn

Java: s.indexOf("x")
来源：http://oiz.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://ybb.shangyingyoupin.top

Ruby: s.index("x")
来源：http://tmn.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://nwa.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eey.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fct.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oic.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hma.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ncw.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vcv.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fsi.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hda.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zhe.dianchejie.cn

[E06] 替换子串
来源：http://nht.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jog.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://mga.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hhl.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://nlo.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfv.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dtl.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pmp.vqdsnc.cn


<!-- 参考信息 -->