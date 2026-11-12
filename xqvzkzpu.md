代发 wailian999

PHP:  // 无重载
来源：http://fzz.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://atw.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://fsm.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ilq.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://uzt.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://gai.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ggo.bbcook.cn

================================================================================
来源：http://hnn.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://drq.fengsongda.top

================================================================================
来源：http://vls.yfazqb.com

[D01] 创建数组 / 列表
来源：http://tfd.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cal.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://syl.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bem.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://zkm.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zku.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://krl.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://nye.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ybb.yfazqb.com

[D02] 追加元素到末尾
来源：http://rpt.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ssx.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cvi.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://vvr.ydzc1.top

TS:   arr.push(4);
来源：http://kyz.ydjk.org.cn

Java: list.add(4);
来源：http://tto.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://uea.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://uyg.jinqigufen.top

C#:   list.Add(4);
来源：http://ujc.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://ikw.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://dxa.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ikt.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cin.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://vrq.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://bje.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://von.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yrz.meibo888.top

C#:   list.Insert(0, 0);
来源：http://kfs.yj202588.top

[D04] 删除元素
来源：http://ovn.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ocz.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pcf.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kej.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://lri.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://irw.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mai.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://obp.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iip.cdnleiting.top

[D05] 访问与修改元素
来源：http://yah.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mkg.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://upg.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cik.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ogb.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://djk.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nua.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://frz.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vsa.sjlbkw.cn

[D06] 数组长度
来源：http://zez.hywenlv.cn

Py:   len(arr)
来源：http://itl.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://fpc.sjlbkw.cn

JS:   arr.length
来源：http://fha.cheryme.top

TS:   arr.length
来源：http://wrq.pengpengdd.cyou

Java: list.size();
来源：http://gxj.aibaodan.cn

Go:   len(arr)
来源：http://zzm.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://ihz.jqgufenzy.top

C#:   list.Count;
来源：http://ztm.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://pcn.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fii.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://hym.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://khp.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://gid.fktsv.cn

Java: list.subList(1, 4);
来源：http://pre.zhoulong.xyz

Go:   arr[1:4]
来源：http://hqa.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://xiu.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://xfa.shzxlz.cn

[D08] 合并两个数组
来源：http://dnb.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://qih.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://sqh.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://itf.chenlongwang.top

TS:   [...a, ...b];
来源：http://hok.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xwm.jlsjyb.cn

Go:   append(a, b...)
来源：http://krc.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://gza.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://xsm.cdnleiting.top

[D09] 排序（升序）
来源：http://iiz.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://upa.yueranfly.top

PHP:  sort($arr);
来源：http://ebq.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tqh.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eyp.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jgx.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xrq.vqdsnc.cn

Ruby: arr.sort
来源：http://owt.cqqwz.cn

C#:   list.Sort();
来源：http://zhs.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aev.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://psg.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzz.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qwr.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dcb.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nmy.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://udw.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ifb.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbw.jianghu66.top

[D11] 反转数组
来源：http://okn.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://jhb.bbcook.cn

PHP:  array_reverse($arr);
来源：http://gfr.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qfl.hammf.cn

TS:   [...arr].reverse();
来源：http://sad.gzhubu.top

Java: Collections.reverse(list);
来源：http://jqy.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://cdd.wangshuangyany.cn

Ruby: arr.reverse
来源：http://lhl.redwolf501.top

C#:   list.Reverse();
来源：http://hrc.ivvv.top

[D12] 查找元素下标
来源：http://wqx.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ulx.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hlk.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpl.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrt.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ves.yonumen.top

Go:   slices.Index(arr, x)
来源：http://zfv.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://nah.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://ftj.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://alc.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://djs.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kts.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://bqq.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://ysd.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xih.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emo.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://mmu.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://utm.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://ecq.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwx.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tuf.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://mks.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://nhz.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gvo.daxiang520.top

Go:   // 手写循环
来源：http://wmo.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://clh.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://zpn.xuetiantiany.cn

[D15] 去重
来源：http://oqx.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftm.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://tmt.yonumen.top

JS:   [...new Set(arr)]
来源：http://ndb.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://evr.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hkg.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aoh.birdmap.top

Ruby: arr.uniq
来源：http://ief.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://jgu.ivvv.top

[D16] 求和与平均值
来源：http://rqz.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qdn.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zce.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dtm.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcf.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aii.jyoumei.cn

Go:   // 手写循环累加
来源：http://apk.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://upd.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://mtv.guannengcc.top

[D17] 最大值与最小值
来源：http://ztb.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://xtl.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://gph.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bfy.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://clw.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://upk.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ija.yj20258.top

Ruby: arr.max;  arr.min
来源：http://gcb.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://uuj.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://adp.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gut.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://azc.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eyc.uphjek.com

TS:   nested.flat();
来源：http://mpl.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://khe.c1oappe.top

Go:   // 手写双层循环
来源：http://tcu.ydzc1.top

Ruby: nested.flatten
来源：http://uvx.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nqs.shzxlz.cn

[D19] 按字段分组
来源：http://qqx.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wbp.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jvj.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vpu.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xgp.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lxr.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://tdo.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qdb.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cob.cashguo.top

[D20] 统计每个元素出现次数
来源：http://taw.jinqigfzy.top

Py:   Counter(arr)
来源：http://avn.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://okb.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvi.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qdx.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://snd.iojbl.cn

Go:   // 手写 map[T]int
来源：http://dso.aizwys.cn

Ruby: arr.tally
来源：http://edq.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sru.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://ylq.zhijiandao.cn

Py:   x in arr
来源：http://mxr.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://aus.xinyue.icu

JS:   arr.includes(x)
来源：http://ojo.sysykeji.top

TS:   arr.includes(x)
来源：http://yzd.jinqigufen.top

Java: list.contains(x)
来源：http://qko.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://gws.xziqi.cn

Ruby: arr.include?(x)
来源：http://axn.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://ujx.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://omj.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://skg.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zal.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gui.yj20258888.top

TS:   [...arr];
来源：http://xia.tarul.cn

Java: new ArrayList<>(list);
来源：http://eqh.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://guf.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://nos.smart0.xyz

C#:   new List<int>(list);
来源：http://mkz.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://vsw.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqs.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mvt.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dry.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvs.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wjb.hcnkem.com

Go:   // 手写循环
来源：http://wpw.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dyb.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bhh.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://bje.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rno.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pew.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://klf.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mei.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bva.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eau.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dcg.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wud.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://xpd.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whc.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://scy.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tkk.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://slw.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pbu.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wfd.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wxt.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://imu.yuanzhike.top

[D26] 数组转字符串
来源：http://gmq.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://bqn.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://igb.cheryme.top

JS:   arr.join(", ")
来源：http://vud.cheryme.top

TS:   arr.join(", ")
来源：http://box.hnxiangtu.top

Java: String.join(", ", list)
来源：http://eji.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://jmf.yongpay.top

Ruby: arr.join(", ")
来源：http://ugq.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://mnn.yongpay.top

================================================================================
来源：http://geq.yanxiufei.cn

E. 字符串处理
来源：http://emg.sjlbkw.cn

================================================================================
来源：http://zww.zhijiandao.cn

[E01] 拼接字符串
来源：http://vqd.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://emp.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vgo.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zqv.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwl.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rie.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ycn.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://plv.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pgl.daria6918.cn

[E02] 重复字符串
来源：http://gls.havefunace.top

Py:   "ab" * 3
来源：http://sti.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://xwe.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://lnd.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://iro.ctjpmb.com

Java: "ab".repeat(3)
来源：http://hzv.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://uay.chenlongwang.top

Ruby: "ab" * 3
来源：http://kxl.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ard.epnwcf.com

[E03] 截取子串
来源：http://fud.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cdn.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oso.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jes.tian-w.cn

TS:   s.slice(1, 4)
来源：http://zes.ivvv.top

Java: s.substring(1, 4)
来源：http://knk.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rij.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://atn.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://gaq.xylfe.cn

[E04] 查找子串位置
来源：http://fqm.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://lzc.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://ogp.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tsw.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://omw.jianghu66.top

Java: s.indexOf("x")
来源：http://vuc.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://tzg.yanxiufei.cn

Ruby: s.index("x")
来源：http://utu.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://aqu.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://alj.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yko.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nsn.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://omr.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://vqt.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blv.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lkp.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://auz.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nag.bbcook.cn

[E06] 替换子串
来源：http://pve.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vfp.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://wis.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdk.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://bxs.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgb.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ubz.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zgl.xylfe.cn


<!-- 参考信息 -->