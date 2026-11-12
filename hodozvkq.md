代发 wailian999

D. 数组 / 列表 / 集合
来源：http://agn.xinyue.icu

================================================================================
来源：http://fcd.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://kty.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lqa.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wwd.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dxm.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uvt.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vrj.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://zrq.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://zoy.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfx.hfpthk.cn

[D02] 追加元素到末尾
来源：http://mtq.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://guk.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jvx.ctjpmb.com

JS:   arr.push(4);
来源：http://csy.xinyue.icu

TS:   arr.push(4);
来源：http://rct.yfazqb.com

Java: list.add(4);
来源：http://ysq.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://vcc.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://fyh.fktsv.cn

C#:   list.Add(4);
来源：http://lao.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://dmk.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://ldy.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vmv.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ndp.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://xua.dianchejie.cn

Java: list.add(0, 0);
来源：http://wbf.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://emn.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vxt.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://jzo.yanxiufei.cn

[D04] 删除元素
来源：http://uwc.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ncc.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aov.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dax.vqdsnc.cn

TS:   arr.splice(0, 1);
来源：http://blw.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ehm.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rum.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dib.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kzl.yueranfly.top

[D05] 访问与修改元素
来源：http://rdi.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jqy.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lbm.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xvv.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://sfs.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://ngf.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://jyd.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kvx.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://atf.dianchejie.cn

[D06] 数组长度
来源：http://hjm.ivvv.top

Py:   len(arr)
来源：http://fzj.bjfxy.top

PHP:  count($arr);
来源：http://obp.tianlin.xyz

JS:   arr.length
来源：http://vgn.birdmap.top

TS:   arr.length
来源：http://zts.pycfn.com

Java: list.size();
来源：http://nwy.fktsv.cn

Go:   len(arr)
来源：http://tow.yj20258.top

Ruby: arr.length; arr.size
来源：http://yjf.cdnleiting.top

C#:   list.Count;
来源：http://vic.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://ugj.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://guw.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://apc.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://mtb.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://knx.cheryme.top

Java: list.subList(1, 4);
来源：http://jby.sjlbkw.cn

Go:   arr[1:4]
来源：http://flm.smart0.xyz

Ruby: arr[1, 3]
来源：http://ewb.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://hsn.jyoumei.cn

[D08] 合并两个数组
来源：http://zmx.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://frm.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://ubl.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://spu.fengsongda.top

TS:   [...a, ...b];
来源：http://opm.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://opq.tianlin.xyz

Go:   append(a, b...)
来源：http://hfk.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://jqu.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://qco.guannengcc.top

[D09] 排序（升序）
来源：http://tbs.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://stj.jqgfzy.top

PHP:  sort($arr);
来源：http://wfi.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gtg.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uxq.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yua.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mtp.ctjpmb.com

Ruby: arr.sort
来源：http://rxl.c1oappe.top

C#:   list.Sort();
来源：http://ypd.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://asp.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qtz.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqd.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlp.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ksg.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyo.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rop.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cmy.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zly.jyoumei.cn

[D11] 反转数组
来源：http://ebl.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://iku.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://loz.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yro.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://hds.ctjpmb.com

Java: Collections.reverse(list);
来源：http://zad.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://vhu.zhengqikj.top

Ruby: arr.reverse
来源：http://huf.jlsjyb.cn

C#:   list.Reverse();
来源：http://qdh.mhx1999.top

[D12] 查找元素下标
来源：http://hll.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://myl.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hkd.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcb.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vsa.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vqm.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://qgu.0kj1m.cn

Ruby: arr.index(x)
来源：http://say.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://fiw.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://nzg.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qna.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pki.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://wms.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://oxs.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zqp.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://opx.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://gml.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mhq.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://nca.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hvh.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jte.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://azs.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://uax.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://gff.jiagoushi.top

Go:   // 手写循环
来源：http://zln.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kiu.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://lyn.zhaomingkeji.xyz

[D15] 去重
来源：http://onn.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fhk.sxryk.cn

PHP:  array_unique($arr);
来源：http://xho.yueranfly.top

JS:   [...new Set(arr)]
来源：http://ezo.yuxming.cn

TS:   [...new Set(arr)]
来源：http://ail.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mos.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://ylm.fengsongda.top

Ruby: arr.uniq
来源：http://nbc.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://gge.zycfv.cn

[D16] 求和与平均值
来源：http://seo.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xwn.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itg.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://phv.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hez.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bmi.zhijiandao.cn

Go:   // 手写循环累加
来源：http://zho.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qcn.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://ppe.hesvh.cn

[D17] 最大值与最小值
来源：http://cxm.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://rbg.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://pfa.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mpl.hfpthk.cn

TS:   Math.max(...arr);
来源：http://eqp.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pje.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://omx.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://xqp.hammf.cn

C#:   list.Max();  list.Min()
来源：http://ehp.316326.xyz

[D18] 扁平化嵌套数组
来源：http://emw.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lco.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://ubm.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qtg.9152youxi.cn

TS:   nested.flat();
来源：http://kqq.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://enj.andypj.xyz

Go:   // 手写双层循环
来源：http://ajp.shuidangran.top

Ruby: nested.flatten
来源：http://dip.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://plb.jyoumei.cn

[D19] 按字段分组
来源：http://wmf.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uyq.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://slw.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yeu.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kcf.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgt.tarul.cn

Go:   // 手写 map[string][]T
来源：http://lki.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tdw.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vxr.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://ncp.hnxiangtu.top

Py:   Counter(arr)
来源：http://pfp.pycfn.com

PHP:  array_count_values($arr);
来源：http://sld.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvz.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jae.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cmg.yongpay.top

Go:   // 手写 map[T]int
来源：http://jll.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://nqn.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pnk.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://adm.chenzaomai.com

Py:   x in arr
来源：http://smo.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://gia.bjfxy.top

JS:   arr.includes(x)
来源：http://aup.ivvv.top

TS:   arr.includes(x)
来源：http://dmu.bbcook.cn

Java: list.contains(x)
来源：http://pgm.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://qst.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://qxr.daxiang520.top

C#:   list.Contains(x)
来源：http://tuq.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://tux.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bsl.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://axy.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vuh.uphjek.com

TS:   [...arr];
来源：http://dqb.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://hqt.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://qtq.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://bgt.snrcjt.cn

C#:   new List<int>(list);
来源：http://qwm.316326.xyz

[D23] reduce 累积计算
来源：http://gwa.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lsx.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lpr.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjx.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gvf.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://asl.chenjidiqi.icu

Go:   // 手写循环
来源：http://bgy.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lxj.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://det.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://pfh.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kgz.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vap.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://krv.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://phr.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yql.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hqi.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fog.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qsx.316326.xyz

[D25] Set 集合去重与交并差
来源：http://gpm.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hyp.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cfz.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mvq.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ouh.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpg.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rmh.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bii.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vmr.xuetiantiany.cn

[D26] 数组转字符串
来源：http://hcv.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://nhq.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://ijs.chenzaomai.com

JS:   arr.join(", ")
来源：http://wwj.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://mzh.xziqi.cn

Java: String.join(", ", list)
来源：http://dif.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://khu.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://vql.hesvh.cn

C#:   string.Join(", ", list)
来源：http://mni.jlsjyb.cn

================================================================================
来源：http://kfk.bjfxy.top

E. 字符串处理
来源：http://fhr.birdmap.top

================================================================================
来源：http://tue.vqdsnc.cn

[E01] 拼接字符串
来源：http://urw.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qgf.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axg.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ull.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbj.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pqn.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vjc.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gxu.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vhr.gzhubu.top

[E02] 重复字符串
来源：http://hpy.9152youxi.cn

Py:   "ab" * 3
来源：http://kox.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://aoz.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://anr.gzhubu.top

TS:   "ab".repeat(3)
来源：http://dud.daria6918.cn

Java: "ab".repeat(3)
来源：http://zbp.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://gjw.sweek.top

Ruby: "ab" * 3
来源：http://jjb.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dtd.yuanzhike.top

[E03] 截取子串
来源：http://yjg.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://avy.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aen.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wac.tanke756.top

TS:   s.slice(1, 4)
来源：http://fnq.dashuyun.cn

Java: s.substring(1, 4)
来源：http://jst.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zme.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://rlc.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://gpl.tarul.cn

[E04] 查找子串位置
来源：http://kiz.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://zkw.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://qji.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mwq.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://nuo.fehbvm.com

Java: s.indexOf("x")
来源：http://wln.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://ogg.dashuyun.cn

Ruby: s.index("x")
来源：http://xis.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://skn.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://szj.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ntx.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qkj.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvd.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dnx.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipx.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mdx.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://roe.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nua.hesvh.cn

[E06] 替换子串
来源：http://rvv.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdp.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://pre.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzn.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://cxn.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://avv.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nwg.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kwd.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://qcb.nanxinkj.top

[E07] 按分隔符拆分
来源：http://ads.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zfp.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://awi.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://zfs.sysykeji.top

TS:   s.split(",")
来源：http://eng.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://kmp.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uue.fktsv.cn


<!-- 参考信息 -->