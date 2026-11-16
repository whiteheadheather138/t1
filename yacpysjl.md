代发 wailian999

PHP:  // 无重载
来源：http://bdh.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mfg.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://hbm.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kzs.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://fzf.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://jcj.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gpw.daria6918.cn

================================================================================
来源：http://qlf.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://mho.dianchejie.cn

================================================================================
来源：http://msg.gzhubu.top

[D01] 创建数组 / 列表
来源：http://gpx.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mxa.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zka.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xty.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gfs.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://njs.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://vrt.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://oyd.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lrj.zycfv.cn

[D02] 追加元素到末尾
来源：http://jie.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rqw.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qdm.yongpay.top

JS:   arr.push(4);
来源：http://ujt.hcnkem.com

TS:   arr.push(4);
来源：http://tij.sufxvd.cn

Java: list.add(4);
来源：http://hfz.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://tfi.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://srh.zhijiandao.cn

C#:   list.Add(4);
来源：http://aws.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://sfr.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://joa.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gbf.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nig.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://cdi.ctjpmb.com

Java: list.add(0, 0);
来源：http://wdq.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://cuo.gaohongyu789.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ibb.hammf.cn

C#:   list.Insert(0, 0);
来源：http://eiv.dianchejie.cn

[D04] 删除元素
来源：http://zrm.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://skw.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bpy.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://flm.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://jik.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ebr.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pwv.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dmv.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wnr.jqgufenzy.top

[D05] 访问与修改元素
来源：http://qut.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qui.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ykp.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hfy.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://uqv.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://fsy.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://pdk.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dxt.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tty.fzhhl.top

[D06] 数组长度
来源：http://poj.shanyushiyangtech.top

Py:   len(arr)
来源：http://jgz.zycfv.cn

PHP:  count($arr);
来源：http://fwy.tarul.cn

JS:   arr.length
来源：http://urr.yongpay.top

TS:   arr.length
来源：http://nlv.hammf.cn

Java: list.size();
来源：http://gxf.sufxvd.cn

Go:   len(arr)
来源：http://fxg.redwolf501.top

Ruby: arr.length; arr.size
来源：http://ufy.shangyingyoupin.top

C#:   list.Count;
来源：http://egq.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://rzc.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nlk.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ztv.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://oho.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://nwe.andypj.xyz

Java: list.subList(1, 4);
来源：http://shy.zhongyouzk.top

Go:   arr[1:4]
来源：http://ngn.tarul.cn

Ruby: arr[1, 3]
来源：http://lon.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://brq.jqgfzy.top

[D08] 合并两个数组
来源：http://gjz.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://mid.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://gam.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vsh.kuanghao11.cn

TS:   [...a, ...b];
来源：http://xnp.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sdl.ydjk.org.cn

Go:   append(a, b...)
来源：http://rvj.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://ghj.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://yrs.jqgfzy.top

[D09] 排序（升序）
来源：http://jlh.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://yoo.birdmap.top

PHP:  sort($arr);
来源：http://gix.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nyq.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://etg.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xmr.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ndb.ivvv.top

Ruby: arr.sort
来源：http://yal.fanxiaobao.xyz

C#:   list.Sort();
来源：http://ggf.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nbr.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nhh.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zjk.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://och.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sow.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtz.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ibo.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lmf.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://omd.tarul.cn

[D11] 反转数组
来源：http://yuk.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jkq.cheryme.top

PHP:  array_reverse($arr);
来源：http://hyv.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cnx.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://ezf.bjfxy.top

Java: Collections.reverse(list);
来源：http://gvr.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://leo.nwbrower.top

Ruby: arr.reverse
来源：http://xvm.zhiwuduotai.top

C#:   list.Reverse();
来源：http://raf.52xcode.cn

[D12] 查找元素下标
来源：http://ljm.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://khc.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://plj.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vqz.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uwb.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ynv.uphjek.com

Go:   slices.Index(arr, x)
来源：http://hbx.tarul.cn

Ruby: arr.index(x)
来源：http://hxo.tarul.cn

C#:   list.IndexOf(x);
来源：http://icl.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://vwe.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zil.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qzh.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://xtb.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://tkh.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fta.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ksw.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qbv.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lkt.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://ubw.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pvl.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kzj.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://xty.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://uqn.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pnv.cheryme.top

Go:   // 手写循环
来源：http://onn.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://bke.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sbh.jinqigfzy.top

[D15] 去重
来源：http://gvx.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lzx.gzhubu.top

PHP:  array_unique($arr);
来源：http://grh.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://gbb.yvedp.cn

TS:   [...new Set(arr)]
来源：http://joe.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://shs.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://muw.chenlongwang.top

Ruby: arr.uniq
来源：http://yqo.pycfn.com

C#:   list.Distinct().ToList()
来源：http://ccl.fehbvm.com

[D16] 求和与平均值
来源：http://kmm.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fmy.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fpa.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pra.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tba.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uyc.zhoulong.xyz

Go:   // 手写循环累加
来源：http://tce.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tjp.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://onx.hesvh.cn

[D17] 最大值与最小值
来源：http://uar.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://qle.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://ffo.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wnj.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://sbc.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cns.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mcp.yonumen.top

Ruby: arr.max;  arr.min
来源：http://gkf.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://aaw.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://erd.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qgi.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://hbq.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vwk.svipenyu.cn

TS:   nested.flat();
来源：http://kcp.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vfh.dashuyun.cn

Go:   // 手写双层循环
来源：http://orf.shzxlz.cn

Ruby: nested.flatten
来源：http://gfg.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://plx.hysaishi.cn

[D19] 按字段分组
来源：http://dao.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ebi.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mga.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bht.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://doc.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://agd.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://pkc.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rbn.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pat.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://rdn.yueranfly.top

Py:   Counter(arr)
来源：http://jir.xuanzx.com

PHP:  array_count_values($arr);
来源：http://ebf.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://plj.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://swx.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jir.tarul.cn

Go:   // 手写 map[T]int
来源：http://yqw.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://esi.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wza.meibo888.top

[D21] 判断是否包含某元素
来源：http://bzp.yueranfly.top

Py:   x in arr
来源：http://lrk.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://dln.kuanghao11.cn

JS:   arr.includes(x)
来源：http://yrz.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://zas.aibaodan.cn

Java: list.contains(x)
来源：http://fxk.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://pyn.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://zrc.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://vum.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://tzk.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://anm.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://grk.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zhx.nwbrower.top

TS:   [...arr];
来源：http://yks.yuxming.cn

Java: new ArrayList<>(list);
来源：http://txr.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://sez.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://ydd.ydzc1.top

C#:   new List<int>(list);
来源：http://cnn.gzhubu.top

[D23] reduce 累积计算
来源：http://qij.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zfb.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ejb.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vcs.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rym.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://suy.vehdjk.com

Go:   // 手写循环
来源：http://fpm.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcc.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://djt.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://hov.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gzr.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xfb.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uuv.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sjq.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lzr.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ngf.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wbn.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://saw.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://sbo.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kgk.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tur.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xsr.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kjn.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uel.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kkh.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yge.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nra.vehdjk.com

[D26] 数组转字符串
来源：http://lua.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://whw.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://ywg.wangdashe.top

JS:   arr.join(", ")
来源：http://jhi.cucudq.cn

TS:   arr.join(", ")
来源：http://mwm.cheryme.top

Java: String.join(", ", list)
来源：http://rlv.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://vzq.fktsv.cn

Ruby: arr.join(", ")
来源：http://xiy.fehbvm.com

C#:   string.Join(", ", list)
来源：http://jgx.xziqi.cn

================================================================================
来源：http://kmf.hysaishi.cn

E. 字符串处理
来源：http://ehq.fanxiaobao.xyz

================================================================================
来源：http://pwm.sysykeji.top

[E01] 拼接字符串
来源：http://cnv.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kmf.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rdl.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://obu.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mmn.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bey.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://skl.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kis.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jpi.gaohongyu789.top

[E02] 重复字符串
来源：http://exf.zhixingplan.top

Py:   "ab" * 3
来源：http://ktx.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://uej.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://cul.fzhhl.top

TS:   "ab".repeat(3)
来源：http://hhb.epnwcf.com

Java: "ab".repeat(3)
来源：http://php.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://aof.zhijiandao.cn

Ruby: "ab" * 3
来源：http://vkz.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uok.tanke756.top

[E03] 截取子串
来源：http://cnv.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://skr.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bqi.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cgj.tanke756.top

TS:   s.slice(1, 4)
来源：http://ino.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://hcy.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbb.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xvw.birdmap.top

C#:   s.Substring(1, 3)
来源：http://agu.xziqi.cn

[E04] 查找子串位置
来源：http://dat.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://znu.pycfn.com

PHP:  strpos($s, "x");
来源：http://ujl.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://der.sufxvd.cn

TS:   s.indexOf("x")
来源：http://tat.vqdsnc.cn

Java: s.indexOf("x")
来源：http://swe.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://gpb.jianghu66.top

Ruby: s.index("x")
来源：http://xkm.gzhubu.top

C#:   s.IndexOf("x")
来源：http://nlv.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cce.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ltu.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zxg.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mrc.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wqe.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pxp.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://clt.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jsz.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pes.cheryme.top

[E06] 替换子串
来源：http://lbe.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gnh.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://rqs.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oit.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://kjp.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fgn.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nlg.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mpl.ctjpmb.com


<!-- 参考信息 -->