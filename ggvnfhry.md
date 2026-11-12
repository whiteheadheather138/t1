代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tro.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ogr.sufxvd.cn

JS:   arr.push(4);
来源：http://ezl.hesvh.cn

TS:   arr.push(4);
来源：http://fgm.meibo888.top

Java: list.add(4);
来源：http://wnm.yongpay.top

Go:   arr = append(arr, 4)
来源：http://lbc.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://nsm.fktsv.cn

C#:   list.Add(4);
来源：http://oim.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://lyo.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://qev.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rsm.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://amw.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://udw.hammf.cn

Java: list.add(0, 0);
来源：http://eiw.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://rvm.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oxr.tanke756.top

C#:   list.Insert(0, 0);
来源：http://mlt.xziqi.cn

[D04] 删除元素
来源：http://wkl.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iqh.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hnh.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qur.yj202588.top

TS:   arr.splice(0, 1);
来源：http://iuf.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://npt.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zym.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fme.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cgy.meibo888.top

[D05] 访问与修改元素
来源：http://eoz.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kvv.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uqt.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nqe.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://mer.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://jnu.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://vhp.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hli.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zhm.zhaomingkeji.xyz

[D06] 数组长度
来源：http://zez.tarul.cn

Py:   len(arr)
来源：http://kog.zhijiandao.cn

PHP:  count($arr);
来源：http://nqv.zhongyouzk.top

JS:   arr.length
来源：http://yqb.pengpengdd.cyou

TS:   arr.length
来源：http://wcg.zdqjudy.top

Java: list.size();
来源：http://haz.svipenyu.cn

Go:   len(arr)
来源：http://uta.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://ccb.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://yqw.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://zno.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://enh.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://poe.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://jqp.yongpay.top

TS:   arr.slice(1, 4);
来源：http://dqj.yangfankeji.com

Java: list.subList(1, 4);
来源：http://xoh.yuanzhike.top

Go:   arr[1:4]
来源：http://xrv.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://nzp.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://zcy.yuanzhike.top

[D08] 合并两个数组
来源：http://mic.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://aec.hammf.cn

PHP:  array_merge($a, $b);
来源：http://dsn.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jbx.fehbvm.com

TS:   [...a, ...b];
来源：http://jni.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qup.ybcxt.top

Go:   append(a, b...)
来源：http://gvk.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://ibw.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://qej.sufxvd.cn

[D09] 排序（升序）
来源：http://ojt.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://mvr.yonumen.top

PHP:  sort($arr);
来源：http://rfl.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://boa.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gvw.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lnw.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bjt.yonumen.top

Ruby: arr.sort
来源：http://cxk.gzhubu.top

C#:   list.Sort();
来源：http://zfn.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tuw.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fub.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zks.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyu.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mrz.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iep.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://inf.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqr.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rmr.hnqzz.top

[D11] 反转数组
来源：http://wes.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://pzy.c1oappe.top

PHP:  array_reverse($arr);
来源：http://lpi.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jwz.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://bgl.hnqzz.top

Java: Collections.reverse(list);
来源：http://vnw.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://zpi.jlsjyb.cn

Ruby: arr.reverse
来源：http://fon.tianlin.xyz

C#:   list.Reverse();
来源：http://hev.tian-w.cn

[D12] 查找元素下标
来源：http://bmz.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://beq.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ipy.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://luc.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yig.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hvf.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://eze.jyoumei.cn

Ruby: arr.index(x)
来源：http://qvt.fzhhl.top

C#:   list.IndexOf(x);
来源：http://wvd.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://jce.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://krt.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pqg.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://wim.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://nfg.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lfc.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jhe.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wkk.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nia.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://zho.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dal.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://awu.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://xlc.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://pcj.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cis.yj20258.top

Go:   // 手写循环
来源：http://wli.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://qrn.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bvz.pycfn.com

[D15] 去重
来源：http://tkt.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pzu.jyoumei.cn

PHP:  array_unique($arr);
来源：http://twp.sysykeji.top

JS:   [...new Set(arr)]
来源：http://qrb.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://hxy.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hbt.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://ruh.shangyingyoupin.top

Ruby: arr.uniq
来源：http://bfi.meibo888.top

C#:   list.Distinct().ToList()
来源：http://okf.zdqjudy.top

[D16] 求和与平均值
来源：http://ehi.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aka.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uzy.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xqr.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rng.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bdx.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://hpu.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fog.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://xck.sysykeji.top

[D17] 最大值与最小值
来源：http://dix.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://xnj.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://qzx.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hpj.nanxinkj.top

TS:   Math.max(...arr);
来源：http://sbs.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vxw.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xrf.birdmap.top

Ruby: arr.max;  arr.min
来源：http://zoj.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://rmh.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://vgv.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ryj.316326.xyz

PHP:  array_merge(...$nested);
来源：http://cpp.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ugx.wangdashe.top

TS:   nested.flat();
来源：http://iac.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zdl.epnwcf.com

Go:   // 手写双层循环
来源：http://tzq.smart0.xyz

Ruby: nested.flatten
来源：http://wtj.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgc.epnwcf.com

[D19] 按字段分组
来源：http://osa.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hnh.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nfp.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://utp.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ebe.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://omv.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://jxo.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qfm.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://llk.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://jjk.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://zzf.yfazqb.com

PHP:  array_count_values($arr);
来源：http://pwe.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nis.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vbm.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gwz.sweek.top

Go:   // 手写 map[T]int
来源：http://ejl.nanxuanxn.top

Ruby: arr.tally
来源：http://vzb.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qnd.epnwcf.com

[D21] 判断是否包含某元素
来源：http://hli.zycfv.cn

Py:   x in arr
来源：http://hny.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://mvp.yongpay.top

JS:   arr.includes(x)
来源：http://xfz.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://qrz.nanxuanxn.top

Java: list.contains(x)
来源：http://fef.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://ibk.hesvh.cn

Ruby: arr.include?(x)
来源：http://mam.aizwys.cn

C#:   list.Contains(x)
来源：http://abl.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://vgd.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dwr.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mnf.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iki.aizwys.cn

TS:   [...arr];
来源：http://htp.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://ttm.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://yno.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://sea.gogol.net.cn

C#:   new List<int>(list);
来源：http://wfy.jianghu66.top

[D23] reduce 累积计算
来源：http://zev.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gvf.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://chx.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://muq.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vnx.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://gcz.zhengqikj.top

Go:   // 手写循环
来源：http://lpu.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pne.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://edz.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://gqp.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gsp.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mkv.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ooo.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hvo.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ytr.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xhv.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://abp.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ixd.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://gin.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gzo.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://icn.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qtd.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nfa.sweek.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://btm.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rch.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://akn.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://prk.uphjek.com

[D26] 数组转字符串
来源：http://zxg.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://pnm.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://vix.sxryk.cn

JS:   arr.join(", ")
来源：http://pzl.sjlbkw.cn

TS:   arr.join(", ")
来源：http://bag.jiagoushi.top

Java: String.join(", ", list)
来源：http://gem.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://jti.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://gnz.meibo888.top

C#:   string.Join(", ", list)
来源：http://ofk.svipenyu.cn

================================================================================
来源：http://xgl.xingfuxueyuan.xyz

E. 字符串处理
来源：http://dlg.tianlin.xyz

================================================================================
来源：http://als.daxiang520.top

[E01] 拼接字符串
来源：http://swg.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lid.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dyi.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zef.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfl.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ebz.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://knh.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://awq.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oyw.jqgfzy.top

[E02] 重复字符串
来源：http://pbm.xuetiantiany.cn

Py:   "ab" * 3
来源：http://xvz.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://ttj.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://tht.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://tpy.shuidangran.top

Java: "ab".repeat(3)
来源：http://zsy.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://ojk.fktsv.cn

Ruby: "ab" * 3
来源：http://gpb.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nha.nanxinkj.top

[E03] 截取子串
来源：http://gbg.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hya.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bki.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://skh.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://znp.cdnleiting.top

Java: s.substring(1, 4)
来源：http://cng.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ccx.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://oxr.yj20258.top

C#:   s.Substring(1, 3)
来源：http://zfg.dashuyun.cn

[E04] 查找子串位置
来源：http://rxp.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://zsn.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://akp.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fgb.sxryk.cn

TS:   s.indexOf("x")
来源：http://kbk.yuxming.cn

Java: s.indexOf("x")
来源：http://zfw.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://tgi.yfazqb.com

Ruby: s.index("x")
来源：http://kwp.guannengcc.top

C#:   s.IndexOf("x")
来源：http://sug.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qrm.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxs.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bcc.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rja.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cmh.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpb.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://riv.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bto.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hzv.jinyuanbaomall.cn

[E06] 替换子串
来源：http://wot.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tqf.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://ybz.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fbi.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://ige.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://drf.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ygd.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kdm.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://goo.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://frz.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hfp.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kvq.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gky.ppjwa.cn

TS:   s.split(",")
来源：http://pcc.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://lec.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qpt.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://ays.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fld.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://ppg.tarul.cn

Py:   ",".join(items)
来源：http://wht.xinyue.icu

PHP:  implode(",", $items);
来源：http://tzl.birdmap.top

JS:   items.join(",")
来源：http://jme.vqdsnc.cn

TS:   items.join(",")
来源：http://kam.feifeiyinyue.top

Java: String.join(",", items)
来源：http://dqc.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://bqn.bbcook.cn

Ruby: items.join(",")
来源：http://jpm.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://mhz.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://uee.cheryme.top


<!-- 参考信息 -->