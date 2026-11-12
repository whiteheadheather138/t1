代发 wailian999

PHP:  // 无重载
来源：http://bsd.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hzl.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://opc.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zps.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://bok.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://yff.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://agk.shuidangran.top

================================================================================
来源：http://mir.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://eeo.hysaishi.cn

================================================================================
来源：http://xbv.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://coz.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://csg.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ckh.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tju.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jeh.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://shw.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://exy.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://nxa.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rhf.cashguo.top

[D02] 追加元素到末尾
来源：http://oqw.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yue.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://keg.daria6918.cn

JS:   arr.push(4);
来源：http://mrv.ehwqpu.com

TS:   arr.push(4);
来源：http://zun.hongshengwenyu.top

Java: list.add(4);
来源：http://yih.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://mpi.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://pgd.yanxiufei.cn

C#:   list.Add(4);
来源：http://gnh.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://fvg.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://jex.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nxc.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhl.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ofb.sweek.top

Java: list.add(0, 0);
来源：http://asc.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://fjh.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cnl.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://ldv.jiagoushi.top

[D04] 删除元素
来源：http://fan.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wtx.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://puf.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wcu.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://ltu.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zuf.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jng.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rab.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://opp.dashuyun.cn

[D05] 访问与修改元素
来源：http://ykx.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hgc.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nfp.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ztu.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://nep.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://gfi.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://niz.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mgz.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ucl.hfpthk.cn

[D06] 数组长度
来源：http://ahx.shuidangran.top

Py:   len(arr)
来源：http://gon.sxryk.cn

PHP:  count($arr);
来源：http://hpf.jinyuanbaomall.cn

JS:   arr.length
来源：http://okl.bbcook.cn

TS:   arr.length
来源：http://ake.bjfxy.top

Java: list.size();
来源：http://iuv.jinghuilouyu.cn

Go:   len(arr)
来源：http://zgt.uphjek.com

Ruby: arr.length; arr.size
来源：http://tiu.yuxming.cn

C#:   list.Count;
来源：http://czs.xinyue.icu

[D07] 切片 / 取子数组
来源：http://sdo.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qpg.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kvc.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://xuk.meibo888.top

TS:   arr.slice(1, 4);
来源：http://ist.zhixingplan.top

Java: list.subList(1, 4);
来源：http://sxc.ydjk.org.cn

Go:   arr[1:4]
来源：http://nzy.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://hzk.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://cav.jqgfzy.top

[D08] 合并两个数组
来源：http://hti.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://zsu.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://gag.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://rze.yuxming.cn

TS:   [...a, ...b];
来源：http://yso.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qdg.nanxuanxn.top

Go:   append(a, b...)
来源：http://wtf.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://yxr.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://ywp.9152youxi.cn

[D09] 排序（升序）
来源：http://qio.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://urk.yuanzhike.top

PHP:  sort($arr);
来源：http://ipo.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://opy.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gyt.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zra.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eev.zhijiandao.cn

Ruby: arr.sort
来源：http://oqg.tanke756.top

C#:   list.Sort();
来源：http://vof.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://axe.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vaw.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnz.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ptq.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wxb.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ted.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wab.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnl.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gdr.yuxming.cn

[D11] 反转数组
来源：http://szf.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ivw.sysykeji.top

PHP:  array_reverse($arr);
来源：http://vcd.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cuk.cucudq.cn

TS:   [...arr].reverse();
来源：http://svs.cucudq.cn

Java: Collections.reverse(list);
来源：http://iht.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://cna.tian-w.cn

Ruby: arr.reverse
来源：http://jkk.ehwqpu.com

C#:   list.Reverse();
来源：http://zsx.yueranfly.top

[D12] 查找元素下标
来源：http://bnb.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://fpz.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xuf.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dfs.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixz.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dmd.pycfn.com

Go:   slices.Index(arr, x)
来源：http://fty.yuxming.cn

Ruby: arr.index(x)
来源：http://sfs.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://zms.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://rmq.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjw.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xap.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://tyi.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://owv.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://upw.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zjc.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wzj.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://lnq.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://lhf.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eja.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xgb.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://oly.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://uqn.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://jxc.cdnleiting.top

Go:   // 手写循环
来源：http://bij.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://lnt.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://xoo.zdbjq.cn

[D15] 去重
来源：http://niu.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ech.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://gfl.tarul.cn

JS:   [...new Set(arr)]
来源：http://gbk.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://uov.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xed.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jih.xuanzx.com

Ruby: arr.uniq
来源：http://qvj.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://gai.316326.xyz

[D16] 求和与平均值
来源：http://mrq.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nqo.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qcn.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogi.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uzq.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://klv.ydzc1.top

Go:   // 手写循环累加
来源：http://lpo.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lnx.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://enp.ybcxt.top

[D17] 最大值与最小值
来源：http://dcx.meibo888.top

Py:   max(arr);  min(arr)
来源：http://epm.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://kzg.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ohx.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://qao.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ktj.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nbh.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://otr.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://juf.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://wqe.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pmi.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://hls.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sxi.shuidangran.top

TS:   nested.flat();
来源：http://rhj.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gky.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://nrv.guannengcc.top

Ruby: nested.flatten
来源：http://wsc.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jab.jinqigufen.top

[D19] 按字段分组
来源：http://man.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hzv.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dqt.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yga.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ket.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://npw.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://ukb.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kyo.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rhx.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://zjw.fzhhl.top

Py:   Counter(arr)
来源：http://zan.iojbl.cn

PHP:  array_count_values($arr);
来源：http://blo.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hrr.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nji.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wal.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://vop.pengpengdd.cyou

Ruby: arr.tally
来源：http://xcu.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vra.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://srd.ydzc1.top

Py:   x in arr
来源：http://lks.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://lkd.ctjpmb.com

JS:   arr.includes(x)
来源：http://kkg.zdbjq.cn

TS:   arr.includes(x)
来源：http://hbo.kuanghao11.cn

Java: list.contains(x)
来源：http://xlj.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://hwo.fzhhl.top

Ruby: arr.include?(x)
来源：http://wbh.haohaochexian.top

C#:   list.Contains(x)
来源：http://shw.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://yvw.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dld.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hek.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vhr.zhijiandao.cn

TS:   [...arr];
来源：http://wdk.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://mkr.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yyz.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://goh.tarul.cn

C#:   new List<int>(list);
来源：http://chi.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://dya.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gax.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://woo.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nlq.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zla.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://roi.yuxming.cn

Go:   // 手写循环
来源：http://jcl.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://opd.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://atc.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://dtp.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://exr.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pdt.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fmg.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://orr.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zpu.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkg.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pvn.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvi.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://csl.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kux.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pvg.svipenyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pal.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bkf.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kzh.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vvs.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mvn.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fkg.shzxlz.cn

[D26] 数组转字符串
来源：http://euz.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://ekr.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://ezn.zhengqikj.top

JS:   arr.join(", ")
来源：http://sjt.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://bgx.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://nnc.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://ikq.gogol.net.cn

Ruby: arr.join(", ")
来源：http://uys.yvedp.cn

C#:   string.Join(", ", list)
来源：http://uyf.smart0.xyz

================================================================================
来源：http://cgx.iojbl.cn

E. 字符串处理
来源：http://pgl.hcnkem.com

================================================================================
来源：http://rdn.pengpengdd.cyou

[E01] 拼接字符串
来源：http://imm.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qqd.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://are.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxg.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqg.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baa.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dzw.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fqh.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wmn.jinqigfzy.top

[E02] 重复字符串
来源：http://iby.yj202588.top

Py:   "ab" * 3
来源：http://ame.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://jek.redwolf501.top

JS:   "ab".repeat(3)
来源：http://plb.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://gvz.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://jsl.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://ouy.kuanghao11.cn

Ruby: "ab" * 3
来源：http://kug.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yxr.iojbl.cn

[E03] 截取子串
来源：http://fyu.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hoo.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lal.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rld.yvedp.cn

TS:   s.slice(1, 4)
来源：http://efm.hysaishi.cn

Java: s.substring(1, 4)
来源：http://bgo.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hwe.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://pcw.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://yox.zycfv.cn

[E04] 查找子串位置
来源：http://zhp.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://alf.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://izg.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jpl.cqqwz.cn

TS:   s.indexOf("x")
来源：http://ydz.sjlbkw.cn

Java: s.indexOf("x")
来源：http://moy.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://ief.guowangkeji.top

Ruby: s.index("x")
来源：http://lez.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://hln.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkm.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dlq.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cnd.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jjt.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lge.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgd.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvb.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://muc.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wwk.tianlin.xyz

[E06] 替换子串
来源：http://ogg.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bcz.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://grp.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wvx.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://fgv.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tzq.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nxg.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ajz.xziqi.cn


<!-- 参考信息 -->