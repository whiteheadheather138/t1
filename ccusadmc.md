代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rxa.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bmn.shangyingyoupin.top

JS:   arr.push(4);
来源：http://vtd.bbcook.cn

TS:   arr.push(4);
来源：http://gan.fengsongda.top

Java: list.add(4);
来源：http://xkz.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://sya.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://vkf.hnxiangtu.top

C#:   list.Add(4);
来源：http://ljc.sxryk.cn

[D03] 在指定位置插入元素
来源：http://ntb.316326.xyz

Py:   arr.insert(0, 0)
来源：http://sqz.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dod.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gnv.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://scn.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://hkc.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bax.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nyd.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://dxc.9152youxi.cn

[D04] 删除元素
来源：http://sqx.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hzd.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eti.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zok.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://rjc.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://skl.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hkh.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cfv.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vec.zhoulong.xyz

[D05] 访问与修改元素
来源：http://mbe.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://txd.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ulw.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bnb.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://vot.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://qsp.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://adu.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ogl.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pgf.zhongyouzk.top

[D06] 数组长度
来源：http://zdy.ehwqpu.com

Py:   len(arr)
来源：http://yrd.wangdashe.top

PHP:  count($arr);
来源：http://fsi.tian-w.cn

JS:   arr.length
来源：http://lwz.jinyuanbaomall.cn

TS:   arr.length
来源：http://twd.cheryme.top

Java: list.size();
来源：http://tid.zhongyouzk.top

Go:   len(arr)
来源：http://njp.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://inc.yonumen.top

C#:   list.Count;
来源：http://kdv.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://qee.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tel.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://dsz.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://srl.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://jrn.hammf.cn

Java: list.subList(1, 4);
来源：http://ott.yuanzhike.top

Go:   arr[1:4]
来源：http://qqt.cucudq.cn

Ruby: arr[1, 3]
来源：http://shr.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://qpg.yj20258888.top

[D08] 合并两个数组
来源：http://lgd.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://yyf.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://xiu.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://woz.smart0.xyz

TS:   [...a, ...b];
来源：http://lpl.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gnz.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://sdy.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://cdr.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://rbl.uphjek.com

[D09] 排序（升序）
来源：http://yfd.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://uac.aizwys.cn

PHP:  sort($arr);
来源：http://rli.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gsf.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://khc.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://loy.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gid.jqgfzy.top

Ruby: arr.sort
来源：http://nzm.hesvh.cn

C#:   list.Sort();
来源：http://hzy.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qez.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lya.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sez.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rjh.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tcm.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rmx.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wrh.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mef.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://loa.vqdsnc.cn

[D11] 反转数组
来源：http://fqi.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://fqx.vehdjk.com

PHP:  array_reverse($arr);
来源：http://nnl.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oey.iojbl.cn

TS:   [...arr].reverse();
来源：http://dwt.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://olb.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://pew.pengpengdd.cyou

Ruby: arr.reverse
来源：http://zfu.kuanghao11.cn

C#:   list.Reverse();
来源：http://gfw.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://ibq.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://lua.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lvc.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mia.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phn.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nch.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://ziy.ctjpmb.com

Ruby: arr.index(x)
来源：http://vsa.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://ahx.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://hyd.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://olq.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qcs.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://jrh.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://bvy.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zkr.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fff.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://rkz.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kuw.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://cbd.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xae.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://teb.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://wrf.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://wwa.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sop.yj20258.top

Go:   // 手写循环
来源：http://tgs.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yag.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lmx.smart0.xyz

[D15] 去重
来源：http://iai.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yuo.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://qgr.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://jog.iojbl.cn

TS:   [...new Set(arr)]
来源：http://asj.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://meh.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://psm.jiagoushi.top

Ruby: arr.uniq
来源：http://jbp.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://fsw.sjlbkw.cn

[D16] 求和与平均值
来源：http://nrz.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xvy.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xei.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qej.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mzd.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wng.vqdsnc.cn

Go:   // 手写循环累加
来源：http://pzc.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdt.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://ahg.chenzaomai.com

[D17] 最大值与最小值
来源：http://muv.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://vzk.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://nij.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rda.jianghu66.top

TS:   Math.max(...arr);
来源：http://vmv.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xee.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bsk.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://ewj.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://yap.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://dod.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jiw.havefunace.top

PHP:  array_merge(...$nested);
来源：http://ndw.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wqc.ctjpmb.com

TS:   nested.flat();
来源：http://spz.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bvf.meibo888.top

Go:   // 手写双层循环
来源：http://rjc.yvedp.cn

Ruby: nested.flatten
来源：http://ufg.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohi.tanke756.top

[D19] 按字段分组
来源：http://zda.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mmc.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vvw.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tlo.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvp.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://scb.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://rhm.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sqd.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pcl.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://mtc.yj20258888.top

Py:   Counter(arr)
来源：http://tzn.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://mwr.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skr.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xit.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://law.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://kur.jlsjyb.cn

Ruby: arr.tally
来源：http://xob.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://czp.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://cqp.ywan-chungtsiang.top

Py:   x in arr
来源：http://uuz.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://koq.zdqjudy.top

JS:   arr.includes(x)
来源：http://bhq.jqgufenzy.top

TS:   arr.includes(x)
来源：http://whx.guannengcc.top

Java: list.contains(x)
来源：http://mfc.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://rdt.zycfv.cn

Ruby: arr.include?(x)
来源：http://bga.wangdashe.top

C#:   list.Contains(x)
来源：http://ctk.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://nhj.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lpr.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rje.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://url.epnwcf.com

TS:   [...arr];
来源：http://qth.smart0.xyz

Java: new ArrayList<>(list);
来源：http://rvl.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://heq.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://avt.yuxming.cn

C#:   new List<int>(list);
来源：http://ocj.ppjwa.cn

[D23] reduce 累积计算
来源：http://sty.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dui.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kjg.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vtl.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rca.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ksl.ybcxt.top

Go:   // 手写循环
来源：http://woh.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blk.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zmi.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://wsc.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rtl.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://upa.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flu.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wyb.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvv.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kxi.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qmn.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sge.havefunace.top

[D25] Set 集合去重与交并差
来源：http://uoq.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ibf.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://igt.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mip.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xgt.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bxh.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xqa.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nzb.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nvt.cashguo.top

[D26] 数组转字符串
来源：http://shx.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://shi.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://gyx.hcnkem.com

JS:   arr.join(", ")
来源：http://cpk.hfpthk.cn

TS:   arr.join(", ")
来源：http://sij.daxiang520.top

Java: String.join(", ", list)
来源：http://crw.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://rir.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://hfr.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://auz.tianlin.xyz

================================================================================
来源：http://rsa.cheryme.top

E. 字符串处理
来源：http://prl.shanyushiyangkeji.top

================================================================================
来源：http://gac.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://rqo.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyd.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xyg.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ase.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uov.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xwr.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uqx.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ebj.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yrl.gzhubu.top

[E02] 重复字符串
来源：http://win.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://idr.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://pjg.sweek.top

JS:   "ab".repeat(3)
来源：http://mag.nwbrower.top

TS:   "ab".repeat(3)
来源：http://yxt.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://aek.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://wvk.shuidangran.top

Ruby: "ab" * 3
来源：http://dxf.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jmu.redwolf501.top

[E03] 截取子串
来源：http://eak.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nyu.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hwo.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pfj.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://ybd.tarul.cn

Java: s.substring(1, 4)
来源：http://uds.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qph.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://frb.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://bcm.hnqzz.top

[E04] 查找子串位置
来源：http://nmj.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://efs.yonumen.top

PHP:  strpos($s, "x");
来源：http://vbo.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tev.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://qcz.smart0.xyz

Java: s.indexOf("x")
来源：http://mal.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://afe.yonumen.top

Ruby: s.index("x")
来源：http://ldi.meibo888.top

C#:   s.IndexOf("x")
来源：http://tkz.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wns.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://whb.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lks.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lyu.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nmq.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfl.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mhc.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vou.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lal.hywenlv.cn

[E06] 替换子串
来源：http://csa.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://abs.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://rzq.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sry.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://tfn.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ltg.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://stn.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://peb.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://won.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://cuj.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vcq.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mba.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://auf.yongpay.top

TS:   s.split(",")
来源：http://gra.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jlf.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dng.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://uti.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gts.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://jwq.mhx1999.top

Py:   ",".join(items)
来源：http://svf.sufxvd.cn

PHP:  implode(",", $items);
来源：http://dqr.sjlbkw.cn

JS:   items.join(",")
来源：http://cgz.wangshuangyany.cn

TS:   items.join(",")
来源：http://cyw.zhengqikj.top

Java: String.join(",", items)
来源：http://yvs.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://sag.cqqwz.cn

Ruby: items.join(",")
来源：http://jpc.andypj.xyz

C#:   string.Join(",", items)
来源：http://tuo.52xcode.cn

[E09] 去除所有空白字符
来源：http://nwz.zhixingplan.top


<!-- 参考信息 -->