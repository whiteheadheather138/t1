代发 wailian999

Ruby: a, b = pair
来源：http://cks.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://fhf.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://zxp.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://txc.yj20258888.top

PHP:  // 无重载
来源：http://efc.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://qja.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://obu.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hry.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://xir.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://enc.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwi.shzxlz.cn

================================================================================
来源：http://wlt.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://vtd.jqgfzy.top

================================================================================
来源：http://hew.xziqi.cn

[D01] 创建数组 / 列表
来源：http://vcv.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ccf.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lmw.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bei.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gyt.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mun.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://ygf.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://huv.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qfk.ybcxt.top

[D02] 追加元素到末尾
来源：http://fsv.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sxu.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nkd.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://dym.hcnkem.com

TS:   arr.push(4);
来源：http://yom.jianghu66.top

Java: list.add(4);
来源：http://lib.uphjek.com

Go:   arr = append(arr, 4)
来源：http://yfd.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://xht.chenjidiqi.icu

C#:   list.Add(4);
来源：http://psr.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://ncv.ivvv.top

Py:   arr.insert(0, 0)
来源：http://czu.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oif.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mig.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://whc.zhongyouzk.top

Java: list.add(0, 0);
来源：http://zvl.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://ixu.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwc.ivvv.top

C#:   list.Insert(0, 0);
来源：http://mda.bbcook.cn

[D04] 删除元素
来源：http://duc.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zjo.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xds.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fat.yonumen.top

TS:   arr.splice(0, 1);
来源：http://jpj.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dsv.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tha.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://quu.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://glr.haohaochexian.top

[D05] 访问与修改元素
来源：http://umk.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vje.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fci.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xhq.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://zsi.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://fah.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://bcc.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sbc.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://muy.ywan-chungtsiang.top

[D06] 数组长度
来源：http://qdc.vqdsnc.cn

Py:   len(arr)
来源：http://jdz.hammf.cn

PHP:  count($arr);
来源：http://yso.kuanghao11.cn

JS:   arr.length
来源：http://aij.yuanzhike.top

TS:   arr.length
来源：http://lyj.birdmap.top

Java: list.size();
来源：http://kew.yfazqb.com

Go:   len(arr)
来源：http://niv.yvedp.cn

Ruby: arr.length; arr.size
来源：http://jea.andypj.xyz

C#:   list.Count;
来源：http://ugl.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://bjt.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aij.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://bdy.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://yqb.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://sqd.0kj1m.cn

Java: list.subList(1, 4);
来源：http://ntb.sufxvd.cn

Go:   arr[1:4]
来源：http://sfr.yonumen.top

Ruby: arr[1, 3]
来源：http://wsy.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://tur.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://nud.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://liq.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://aej.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xee.redwolf501.top

TS:   [...a, ...b];
来源：http://ffy.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zvp.fehbvm.com

Go:   append(a, b...)
来源：http://cmt.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://gxq.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://bor.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://avk.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://hru.gogol.net.cn

PHP:  sort($arr);
来源：http://edh.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qwv.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://ktk.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lqm.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iam.cucudq.cn

Ruby: arr.sort
来源：http://nsl.xziqi.cn

C#:   list.Sort();
来源：http://jix.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://igs.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ymp.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vkc.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://egz.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fov.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://psh.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mkr.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yeg.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tzo.gaohongyu789.top

[D11] 反转数组
来源：http://pow.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://gee.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://pbd.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tpa.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://ebx.yfazqb.com

Java: Collections.reverse(list);
来源：http://oqp.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://chz.bbcook.cn

Ruby: arr.reverse
来源：http://toz.jinqigufen.top

C#:   list.Reverse();
来源：http://pig.yj202588.top

[D12] 查找元素下标
来源：http://byb.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://ocs.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fop.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqr.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gbb.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wzp.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://xof.zhongyouzk.top

Ruby: arr.index(x)
来源：http://dfp.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://qrg.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://vfo.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cbf.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://llv.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://fra.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://qpx.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fse.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nuv.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://fmo.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fcs.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://neu.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wds.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ttt.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://yin.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://ljb.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://inr.svipenyu.cn

Go:   // 手写循环
来源：http://omv.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://zyk.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fai.jqgfzy.top

[D15] 去重
来源：http://wxj.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://csp.cheryme.top

PHP:  array_unique($arr);
来源：http://pah.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://uzx.yuxming.cn

TS:   [...new Set(arr)]
来源：http://yxv.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dqf.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://gcb.aizwys.cn

Ruby: arr.uniq
来源：http://avt.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://hfl.wangshuangyany.cn

[D16] 求和与平均值
来源：http://vcb.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jty.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://par.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jhl.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyj.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rbf.zhoulong.xyz

Go:   // 手写循环累加
来源：http://yxw.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://smi.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://cvm.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://khn.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://bnf.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://jth.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ibo.meibo888.top

TS:   Math.max(...arr);
来源：http://tqp.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aiy.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vul.yj202588.top

Ruby: arr.max;  arr.min
来源：http://nfj.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://jtn.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://uhh.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xyk.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://fre.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gug.zhiwuduotai.top

TS:   nested.flat();
来源：http://lpr.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kmw.yj20258.top

Go:   // 手写双层循环
来源：http://ono.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://aao.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hww.316326.xyz

[D19] 按字段分组
来源：http://hbb.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wod.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://icj.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpe.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yeh.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aht.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://zzv.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dbr.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nxq.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://cji.nwbrower.top

Py:   Counter(arr)
来源：http://ckt.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://iug.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lod.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pui.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://khe.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://qkh.hnxiangtu.top

Ruby: arr.tally
来源：http://lbf.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vvb.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://rhn.cdnleiting.top

Py:   x in arr
来源：http://bqp.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://mac.9152youxi.cn

JS:   arr.includes(x)
来源：http://euo.svipenyu.cn

TS:   arr.includes(x)
来源：http://zol.aibaodan.cn

Java: list.contains(x)
来源：http://qpe.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://eea.52xcode.cn

Ruby: arr.include?(x)
来源：http://rnc.hnqzz.top

C#:   list.Contains(x)
来源：http://kov.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://yhw.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kqd.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zsn.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hzf.0kj1m.cn

TS:   [...arr];
来源：http://lbm.cucudq.cn

Java: new ArrayList<>(list);
来源：http://dam.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bdz.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://haz.bbcook.cn

C#:   new List<int>(list);
来源：http://mqw.zhixingplan.top

[D23] reduce 累积计算
来源：http://ose.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pml.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eki.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://unc.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zae.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fnv.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://log.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nhy.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iqo.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://krx.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tub.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vlu.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpe.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dde.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sue.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jrp.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xsl.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://doo.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://frz.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://flg.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bbw.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qnw.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://upn.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zov.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xvs.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mff.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wel.9152youxi.cn

[D26] 数组转字符串
来源：http://ncs.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://riq.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://gpu.gzhubu.top

JS:   arr.join(", ")
来源：http://bjz.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://pok.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://kaa.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://crl.zhengqikj.top

Ruby: arr.join(", ")
来源：http://lur.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://bav.jianghu66.top

================================================================================
来源：http://ofg.shanyushiyangkeji.top

E. 字符串处理
来源：http://drl.ybcxt.top

================================================================================
来源：http://scz.cashguo.top

[E01] 拼接字符串
来源：http://rxd.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ump.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpx.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xua.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ntu.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vkg.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yoe.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vcp.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjh.tianlin.xyz

[E02] 重复字符串
来源：http://upg.guannengcc.top

Py:   "ab" * 3
来源：http://cyj.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://shm.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://qoe.yj20258888.top

TS:   "ab".repeat(3)
来源：http://ula.zhengqikj.top

Java: "ab".repeat(3)
来源：http://arx.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://lro.zhengqikj.top

Ruby: "ab" * 3
来源：http://xtn.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mch.yj20258888.top

[E03] 截取子串
来源：http://ruc.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wpr.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qes.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqi.cheryme.top

TS:   s.slice(1, 4)
来源：http://ofb.hesvh.cn

Java: s.substring(1, 4)
来源：http://lys.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ald.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://lnw.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://ein.zhengqikj.top

[E04] 查找子串位置
来源：http://zco.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://ack.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://nbx.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yab.hcnkem.com

TS:   s.indexOf("x")
来源：http://mcb.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://irl.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://pug.tarul.cn

Ruby: s.index("x")
来源：http://oho.aizwys.cn

C#:   s.IndexOf("x")
来源：http://bih.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qpw.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ftz.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eqt.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fln.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ysc.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uwg.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gmp.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ncz.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fms.fehbvm.com

[E06] 替换子串
来源：http://nyq.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mha.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://wlc.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckr.jianghu66.top


<!-- 参考信息 -->