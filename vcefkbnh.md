代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ksz.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ipq.cdnleiting.top

Java: // 无解构
来源：http://pzx.cucudq.cn

Go:   // 无解构
来源：http://xjl.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://dob.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://kxl.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://hmy.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://whl.yj20258.top

PHP:  // 无重载
来源：http://dau.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://smt.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://jbs.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cfk.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://eoc.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://vie.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://shx.jinqigfzy.top

================================================================================
来源：http://cjh.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://iql.jyoumei.cn

================================================================================
来源：http://iat.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://mlx.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://her.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://efe.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgw.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://stl.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qno.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://cyi.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://fkh.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ydf.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://lbo.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xtd.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cjw.daxiang520.top

JS:   arr.push(4);
来源：http://mkv.hammf.cn

TS:   arr.push(4);
来源：http://ejn.yuxming.cn

Java: list.add(4);
来源：http://yrd.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://nqy.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://hmo.0kj1m.cn

C#:   list.Add(4);
来源：http://abz.cheryme.top

[D03] 在指定位置插入元素
来源：http://ors.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://xyu.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ztr.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gtl.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://tat.aibaodan.cn

Java: list.add(0, 0);
来源：http://dos.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tro.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ljf.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://pcj.pycfn.com

[D04] 删除元素
来源：http://tax.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ong.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uyh.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xso.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://cri.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iwb.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yal.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjg.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sff.zdqjudy.top

[D05] 访问与修改元素
来源：http://cnh.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zpb.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hbp.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fee.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://uar.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://yan.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://wjc.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fgx.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://drp.snrcjt.cn

[D06] 数组长度
来源：http://wka.jyoumei.cn

Py:   len(arr)
来源：http://qnz.snrcjt.cn

PHP:  count($arr);
来源：http://xvf.shanyushiyangtech.top

JS:   arr.length
来源：http://ddk.hnxiangtu.top

TS:   arr.length
来源：http://fji.tanke756.top

Java: list.size();
来源：http://wfq.316326.xyz

Go:   len(arr)
来源：http://bfw.sxryk.cn

Ruby: arr.length; arr.size
来源：http://hqh.guannengcc.top

C#:   list.Count;
来源：http://yee.andypj.xyz

[D07] 切片 / 取子数组
来源：http://exz.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://esl.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qwd.316326.xyz

JS:   arr.slice(1, 4);
来源：http://aqu.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://uvb.zdqjudy.top

Java: list.subList(1, 4);
来源：http://xfb.cdnleiting.top

Go:   arr[1:4]
来源：http://cjy.hammf.cn

Ruby: arr[1, 3]
来源：http://hzi.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://jci.zhongyouzk.top

[D08] 合并两个数组
来源：http://slg.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://ksh.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://cmn.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ghh.ydjk.org.cn

TS:   [...a, ...b];
来源：http://apr.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pwf.ydjk.org.cn

Go:   append(a, b...)
来源：http://dai.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://xkn.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://zae.quarkkingdee.top

[D09] 排序（升序）
来源：http://smy.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://hha.zhiwuduotai.top

PHP:  sort($arr);
来源：http://eeu.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lqw.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://bem.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://khy.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://few.shanyushiyangtech.top

Ruby: arr.sort
来源：http://mvx.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://eib.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wxy.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mjj.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwa.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xse.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnr.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cll.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dje.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nok.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oys.jyoumei.cn

[D11] 反转数组
来源：http://ueb.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zic.yj20258888.top

PHP:  array_reverse($arr);
来源：http://sow.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pnd.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://shx.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://wbg.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://zzj.52xcode.cn

Ruby: arr.reverse
来源：http://tug.sufxvd.cn

C#:   list.Reverse();
来源：http://llp.ydjk.org.cn

[D12] 查找元素下标
来源：http://hul.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://aes.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xwt.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://huc.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcp.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fel.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://qdj.yuxming.cn

Ruby: arr.index(x)
来源：http://vxy.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://flb.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://gda.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fgv.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uwf.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://ojf.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://css.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://imb.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sqb.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://mws.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hxd.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://jmo.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lda.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bul.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://eds.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://tzm.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zvb.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://cyi.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bfo.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lva.redwolf501.top

[D15] 去重
来源：http://vfb.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yki.dashuyun.cn

PHP:  array_unique($arr);
来源：http://iir.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://eqf.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://vkt.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hln.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cor.bbcook.cn

Ruby: arr.uniq
来源：http://yut.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://dmv.hywenlv.cn

[D16] 求和与平均值
来源：http://cnq.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayn.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lti.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://btv.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://syy.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xkf.9152youxi.cn

Go:   // 手写循环累加
来源：http://onp.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqm.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://ccl.hfpthk.cn

[D17] 最大值与最小值
来源：http://wby.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://llr.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://djt.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lyg.tian-w.cn

TS:   Math.max(...arr);
来源：http://etc.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hpz.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://umy.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://mwj.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://iog.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://sye.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tyw.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://bjt.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://njh.jinghuilouyu.cn

TS:   nested.flat();
来源：http://ujm.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kib.tanke756.top

Go:   // 手写双层循环
来源：http://hud.andypj.xyz

Ruby: nested.flatten
来源：http://cle.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dym.yangfankeji.com

[D19] 按字段分组
来源：http://tom.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dbi.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yot.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wll.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cwl.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://srt.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://mwo.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uhk.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bfx.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://smk.guowangkeji.top

Py:   Counter(arr)
来源：http://cws.yongpay.top

PHP:  array_count_values($arr);
来源：http://vdv.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pfi.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yie.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xdm.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://ncm.shanyushiyangtech.top

Ruby: arr.tally
来源：http://hus.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rht.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://rza.xuetiantiany.cn

Py:   x in arr
来源：http://abi.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://aop.guannengcc.top

JS:   arr.includes(x)
来源：http://jfr.bbcook.cn

TS:   arr.includes(x)
来源：http://uvk.zhengqikj.top

Java: list.contains(x)
来源：http://mdc.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://vyo.yj20258.top

Ruby: arr.include?(x)
来源：http://oxd.fengsongda.top

C#:   list.Contains(x)
来源：http://ule.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://fnm.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ygf.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://euy.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nxt.iojbl.cn

TS:   [...arr];
来源：http://ies.fzhhl.top

Java: new ArrayList<>(list);
来源：http://had.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://ibx.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://yiw.ctjpmb.com

C#:   new List<int>(list);
来源：http://duk.yj20258.top

[D23] reduce 累积计算
来源：http://ktw.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eyq.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://njm.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://haf.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcn.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fqv.cqqwz.cn

Go:   // 手写循环
来源：http://ppe.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://srl.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gjd.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://rbx.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jae.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xqt.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xpz.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wmv.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ial.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgl.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vau.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oag.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://ygd.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cqk.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ujo.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ykc.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xbr.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aey.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wrn.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tno.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://olf.dianchejie.cn

[D26] 数组转字符串
来源：http://chz.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://aur.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://lci.xziqi.cn

JS:   arr.join(", ")
来源：http://mqp.xinyue.icu

TS:   arr.join(", ")
来源：http://pss.yuanzhike.top

Java: String.join(", ", list)
来源：http://rxk.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://aoq.shzxlz.cn

Ruby: arr.join(", ")
来源：http://liv.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://hxw.shanyushiyangkeji.top

================================================================================
来源：http://xgm.xinyue.icu

E. 字符串处理
来源：http://dce.pengpengdd.cyou

================================================================================
来源：http://szh.shuidangran.top

[E01] 拼接字符串
来源：http://sfu.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zqv.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blp.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://umg.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hry.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xln.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://brc.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jhh.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ojg.xuanzx.com

[E02] 重复字符串
来源：http://yvq.yj20258888.top

Py:   "ab" * 3
来源：http://ace.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://ckr.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://fva.yongpay.top

TS:   "ab".repeat(3)
来源：http://avo.hfpthk.cn

Java: "ab".repeat(3)
来源：http://zip.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://rnk.zhixingplan.top

Ruby: "ab" * 3
来源：http://mqw.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nkv.smart0.xyz

[E03] 截取子串
来源：http://wfp.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oka.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://whh.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xgt.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://jhl.dianchejie.cn

Java: s.substring(1, 4)
来源：http://kum.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jyr.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fba.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://unx.cucudq.cn

[E04] 查找子串位置
来源：http://fxu.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://pgg.cucudq.cn

PHP:  strpos($s, "x");
来源：http://jwg.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zai.xuanzx.com

TS:   s.indexOf("x")
来源：http://tti.yvedp.cn

Java: s.indexOf("x")
来源：http://piu.uphjek.com

Go:   strings.Index(s, "x")
来源：http://fqq.zdqjudy.top

Ruby: s.index("x")
来源：http://zpe.guannengcc.top

C#:   s.IndexOf("x")
来源：http://fmk.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgc.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wuz.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ryn.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emi.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kzu.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wiv.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dnd.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gci.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cac.aizwys.cn


<!-- 参考信息 -->