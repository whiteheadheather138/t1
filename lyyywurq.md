代发 wailian999

PHP:  // 无重载
来源：http://mri.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xsh.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://jwv.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://azs.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://ljw.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://jxf.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rde.uphjek.com

================================================================================
来源：http://xni.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://pvg.cashguo.top

================================================================================
来源：http://jib.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://kpz.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://ahe.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ygg.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pry.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://alv.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gme.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://sfl.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://qny.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wim.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://nzk.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://azu.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vnf.pengpengdd.cyou

JS:   arr.push(4);
来源：http://woj.cqqwz.cn

TS:   arr.push(4);
来源：http://xkd.cashguo.top

Java: list.add(4);
来源：http://pqv.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://ldh.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://ydg.ybcxt.top

C#:   list.Add(4);
来源：http://dmc.meibo888.top

[D03] 在指定位置插入元素
来源：http://eap.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://tbp.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zhn.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vxa.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://yjk.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://sjh.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://ujv.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xvp.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://hdz.yj20258888.top

[D04] 删除元素
来源：http://iag.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hjf.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cuv.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uiy.havefunace.top

TS:   arr.splice(0, 1);
来源：http://xrg.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgh.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dev.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dhr.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hqj.ctjpmb.com

[D05] 访问与修改元素
来源：http://ntp.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://afp.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yex.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://grk.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://wgu.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://tse.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://edi.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjm.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hge.haohaochexian.top

[D06] 数组长度
来源：http://mxn.c1oappe.top

Py:   len(arr)
来源：http://xad.jianghu66.top

PHP:  count($arr);
来源：http://ioc.fehbvm.com

JS:   arr.length
来源：http://bbz.xziqi.cn

TS:   arr.length
来源：http://lgl.uphjek.com

Java: list.size();
来源：http://wnb.hongshengwenyu.top

Go:   len(arr)
来源：http://hcb.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://zpp.tian-w.cn

C#:   list.Count;
来源：http://zol.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://ruy.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rdk.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qer.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://hxt.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://sbr.hammf.cn

Java: list.subList(1, 4);
来源：http://lxm.aibaodan.cn

Go:   arr[1:4]
来源：http://ghs.jianghu66.top

Ruby: arr[1, 3]
来源：http://ywu.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://xpz.yvedp.cn

[D08] 合并两个数组
来源：http://fpn.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://kdr.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://ean.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cro.hfpthk.cn

TS:   [...a, ...b];
来源：http://dhz.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://caa.epnwcf.com

Go:   append(a, b...)
来源：http://yqp.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://pxw.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://bxu.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://xjr.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://fkf.nanxinkj.top

PHP:  sort($arr);
来源：http://lax.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wxo.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kyl.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://his.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfu.gotoacloud.top

Ruby: arr.sort
来源：http://nif.ppjwa.cn

C#:   list.Sort();
来源：http://dhg.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xoc.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pdj.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpj.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wuv.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lit.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dzp.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zhn.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://onp.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://erl.iojbl.cn

[D11] 反转数组
来源：http://udn.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://rno.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://eih.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kzh.xylfe.cn

TS:   [...arr].reverse();
来源：http://wkm.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://haz.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://ozk.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://qis.chenzaomai.com

C#:   list.Reverse();
来源：http://hft.hcnkem.com

[D12] 查找元素下标
来源：http://gzq.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://ptd.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wye.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdo.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pwo.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hpv.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://woy.cashguo.top

Ruby: arr.index(x)
来源：http://xpq.yuxming.cn

C#:   list.IndexOf(x);
来源：http://xpr.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://mlc.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://egx.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bro.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://kji.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://hns.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kob.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hrg.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://bpy.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkg.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://kee.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kef.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lob.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://xwr.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://yss.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfo.epnwcf.com

Go:   // 手写循环
来源：http://ayy.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tcl.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lbf.shangyingyoupin.top

[D15] 去重
来源：http://ytx.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ywd.ehwqpu.com

PHP:  array_unique($arr);
来源：http://ycd.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://vfn.yj202588.top

TS:   [...new Set(arr)]
来源：http://gfx.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hgp.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cqf.birdmap.top

Ruby: arr.uniq
来源：http://zii.birdmap.top

C#:   list.Distinct().ToList()
来源：http://fwl.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://cda.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqq.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gwj.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdd.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibh.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://spm.daxiang520.top

Go:   // 手写循环累加
来源：http://evr.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oee.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://jyq.vqdsnc.cn

[D17] 最大值与最小值
来源：http://inw.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://qpm.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://lkc.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pti.tanke756.top

TS:   Math.max(...arr);
来源：http://swj.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oru.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dkd.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://qzj.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://mvc.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://ylk.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gat.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://xnj.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uay.sjlbkw.cn

TS:   nested.flat();
来源：http://wfn.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iag.yongpay.top

Go:   // 手写双层循环
来源：http://vln.sysykeji.top

Ruby: nested.flatten
来源：http://rhu.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ikr.ivvv.top

[D19] 按字段分组
来源：http://lop.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jxj.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lcy.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gvp.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cto.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzo.316326.xyz

Go:   // 手写 map[string][]T
来源：http://epf.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ret.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vad.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://wfm.bbcook.cn

Py:   Counter(arr)
来源：http://uhp.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://mwl.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzt.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lcp.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zvs.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://inm.yuxming.cn

Ruby: arr.tally
来源：http://qhi.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xwz.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://ojr.hnxiangtu.top

Py:   x in arr
来源：http://ice.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://isb.daria6918.cn

JS:   arr.includes(x)
来源：http://mhz.uphjek.com

TS:   arr.includes(x)
来源：http://fuj.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://jfk.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://wed.cashguo.top

Ruby: arr.include?(x)
来源：http://irq.316326.xyz

C#:   list.Contains(x)
来源：http://wgz.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://oxw.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hvf.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qaa.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vgg.yueranfly.top

TS:   [...arr];
来源：http://dxv.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://rnp.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://shp.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://rms.cucudq.cn

C#:   new List<int>(list);
来源：http://iwy.zhixingplan.top

[D23] reduce 累积计算
来源：http://xkr.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zxl.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ipn.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvy.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axe.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fyo.daria6918.cn

Go:   // 手写循环
来源：http://tay.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://efb.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctg.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://feq.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hja.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jnx.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rcg.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dhs.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dkr.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldc.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lve.jinqigfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://knh.hammf.cn

[D25] Set 集合去重与交并差
来源：http://ncu.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gzq.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mrp.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tph.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vip.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lqs.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xbm.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zhf.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rcr.wangshuangyany.cn

[D26] 数组转字符串
来源：http://yhx.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://ylx.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://hio.yj20258.top

JS:   arr.join(", ")
来源：http://wsj.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://ymb.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://apc.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://lko.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://pft.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://nwg.ydzc1.top

================================================================================
来源：http://pvg.zhoulong.xyz

E. 字符串处理
来源：http://uww.jinqigfzy.top

================================================================================
来源：http://irg.cheryme.top

[E01] 拼接字符串
来源：http://odl.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pdu.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vtg.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofd.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://duu.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqh.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ykp.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kan.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://icc.dashuyun.cn

[E02] 重复字符串
来源：http://vzr.chenjidiqi.icu

Py:   "ab" * 3
来源：http://tzm.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://wom.uphjek.com

JS:   "ab".repeat(3)
来源：http://hfb.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://dby.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://sat.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://qhj.hcnkem.com

Ruby: "ab" * 3
来源：http://uvy.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xyg.bbcook.cn

[E03] 截取子串
来源：http://dla.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvi.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://evn.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dis.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://qsf.gotoacloud.top

Java: s.substring(1, 4)
来源：http://ffa.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tbk.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://dpk.uphjek.com

C#:   s.Substring(1, 3)
来源：http://wrl.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://zxa.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://tig.cheryme.top

PHP:  strpos($s, "x");
来源：http://lrk.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ylv.hnqzz.top

TS:   s.indexOf("x")
来源：http://ghn.gaohongyu789.top

Java: s.indexOf("x")
来源：http://uur.yongpay.top

Go:   strings.Index(s, "x")
来源：http://hhn.iojbl.cn

Ruby: s.index("x")
来源：http://mtb.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://vso.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dwn.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lfn.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vqq.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prj.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xia.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wdt.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bqb.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zrr.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dre.chenlongwang.top

[E06] 替换子串
来源：http://esu.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvf.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://eni.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uyi.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://mjz.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zdj.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://spm.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://idi.nanxuanxn.top


<!-- 参考信息 -->