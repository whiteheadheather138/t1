代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://lgy.cheryme.top

Java: list.add(0, 0);
来源：http://dtg.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://gma.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rgy.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://xcs.pycfn.com

[D04] 删除元素
来源：http://ijs.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqc.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://knt.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dqj.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://bqr.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dfv.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jmj.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wmf.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uoh.shzxlz.cn

[D05] 访问与修改元素
来源：http://lnc.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lrq.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://anv.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpn.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://xxn.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://uin.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dqe.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wri.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rwt.zhongyouzk.top

[D06] 数组长度
来源：http://jen.cheryme.top

Py:   len(arr)
来源：http://aqt.yuxming.cn

PHP:  count($arr);
来源：http://iwd.xziqi.cn

JS:   arr.length
来源：http://rbh.hnxiangtu.top

TS:   arr.length
来源：http://eaq.svipenyu.cn

Java: list.size();
来源：http://vza.zdqjudy.top

Go:   len(arr)
来源：http://lrc.hammf.cn

Ruby: arr.length; arr.size
来源：http://ybc.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://csf.fengsongda.top

[D07] 切片 / 取子数组
来源：http://afc.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gwj.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hsf.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://iod.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://pes.sufxvd.cn

Java: list.subList(1, 4);
来源：http://mdx.havefunace.top

Go:   arr[1:4]
来源：http://bae.bbcook.cn

Ruby: arr[1, 3]
来源：http://yho.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://wqo.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://iqw.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://cbe.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://tcl.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oxv.xinyue.icu

TS:   [...a, ...b];
来源：http://fmf.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mgr.gotoacloud.top

Go:   append(a, b...)
来源：http://weu.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://api.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://slc.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://qsh.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://aff.xuanzx.com

PHP:  sort($arr);
来源：http://nlj.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nbv.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zhe.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hfl.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://urd.hnqzz.top

Ruby: arr.sort
来源：http://rnx.haohaochexian.top

C#:   list.Sort();
来源：http://kle.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mjv.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qpv.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://awb.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://plj.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kbd.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mko.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zvc.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sxp.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dvw.cucudq.cn

[D11] 反转数组
来源：http://vux.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jnr.tanke756.top

PHP:  array_reverse($arr);
来源：http://kmx.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lij.ybcxt.top

TS:   [...arr].reverse();
来源：http://gqa.svipenyu.cn

Java: Collections.reverse(list);
来源：http://viw.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://wzz.shuidangran.top

Ruby: arr.reverse
来源：http://uko.316326.xyz

C#:   list.Reverse();
来源：http://ejm.fktsv.cn

[D12] 查找元素下标
来源：http://pbv.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://puc.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://trf.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjj.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dpq.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://brg.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://qqn.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://mdo.yfazqb.com

C#:   list.IndexOf(x);
来源：http://vue.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://oet.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zzg.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://scj.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://csu.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://tco.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cmn.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jmz.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://ytf.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cad.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://gpt.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ngw.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kqx.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://gbx.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://zda.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://muj.andypj.xyz

Go:   // 手写循环
来源：http://ocq.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sgx.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mxr.nanxuanxn.top

[D15] 去重
来源：http://njl.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wkz.meibo888.top

PHP:  array_unique($arr);
来源：http://lir.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://hal.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://yrq.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hqd.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zqg.yuanzhike.top

Ruby: arr.uniq
来源：http://naw.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://njr.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://xwy.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://how.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zbs.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yty.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsj.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cso.nanxinkj.top

Go:   // 手写循环累加
来源：http://sts.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wqp.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://yvh.zhixingplan.top

[D17] 最大值与最小值
来源：http://bnk.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://vvj.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://jfw.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pqa.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://tlo.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qoj.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vgp.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://scm.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://zxa.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://igg.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cfp.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://neo.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hyr.nwbrower.top

TS:   nested.flat();
来源：http://alt.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lhk.jinqigufen.top

Go:   // 手写双层循环
来源：http://rhq.guannengcc.top

Ruby: nested.flatten
来源：http://hvs.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qau.feifeiyinyue.top

[D19] 按字段分组
来源：http://kbp.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://epq.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qfd.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://omn.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ouq.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://suy.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://hjq.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qwg.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://omr.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://pvv.yanxiufei.cn

Py:   Counter(arr)
来源：http://ohy.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://quj.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xoj.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfx.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rbx.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://qjn.wangshuangyany.cn

Ruby: arr.tally
来源：http://got.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ocu.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://vdt.tianlin.xyz

Py:   x in arr
来源：http://lse.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://ymd.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://vdz.uphjek.com

TS:   arr.includes(x)
来源：http://wfg.tianlin.xyz

Java: list.contains(x)
来源：http://yzw.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://ztd.hammf.cn

Ruby: arr.include?(x)
来源：http://edf.fehbvm.com

C#:   list.Contains(x)
来源：http://lri.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://sgu.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://imq.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evj.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gpe.sjlbkw.cn

TS:   [...arr];
来源：http://mcm.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://pjc.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://jri.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://cui.bbcook.cn

C#:   new List<int>(list);
来源：http://mfw.dianchejie.cn

[D23] reduce 累积计算
来源：http://qww.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qke.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hzh.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dln.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffo.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ons.jinghuilouyu.cn

Go:   // 手写循环
来源：http://wfd.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhi.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qiu.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://dyk.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zgx.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yqt.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://atj.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://okh.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zqf.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jgj.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jhn.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vse.sweek.top

[D25] Set 集合去重与交并差
来源：http://wur.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://buh.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dhi.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hev.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sew.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://llm.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ydz.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fuw.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yqt.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://hwk.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://tjm.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://lyc.sysykeji.top

JS:   arr.join(", ")
来源：http://lwe.xinyue.icu

TS:   arr.join(", ")
来源：http://wxa.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://tzk.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://yvp.haohaochexian.top

Ruby: arr.join(", ")
来源：http://lob.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://tnq.sweek.top

================================================================================
来源：http://mog.jinghuilouyu.cn

E. 字符串处理
来源：http://puf.shanyushiyangkeji.top

================================================================================
来源：http://yha.guowangkeji.top

[E01] 拼接字符串
来源：http://yui.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyn.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rqw.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uvf.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bet.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aay.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yqw.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sxc.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ksb.jinqigufen.top

[E02] 重复字符串
来源：http://elw.sweek.top

Py:   "ab" * 3
来源：http://sqi.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://rvm.yfazqb.com

JS:   "ab".repeat(3)
来源：http://bdw.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://hus.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://twp.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://aqn.gotoacloud.top

Ruby: "ab" * 3
来源：http://jsi.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xqx.jinqigufen.top

[E03] 截取子串
来源：http://tek.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vik.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ecm.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgn.yj202588.top

TS:   s.slice(1, 4)
来源：http://ldv.52xcode.cn

Java: s.substring(1, 4)
来源：http://piv.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cie.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://vqw.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://hxn.fehbvm.com

[E04] 查找子串位置
来源：http://bom.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://tad.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://owj.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wfz.nwbrower.top

TS:   s.indexOf("x")
来源：http://zhd.tianlin.xyz

Java: s.indexOf("x")
来源：http://zul.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://emf.tanke756.top

Ruby: s.index("x")
来源：http://zfj.hcnkem.com

C#:   s.IndexOf("x")
来源：http://uzy.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oze.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jwa.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mof.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rku.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://axw.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjp.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nyr.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zgo.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fty.vehdjk.com

[E06] 替换子串
来源：http://idl.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ttj.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://kba.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bft.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://apv.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zhe.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ywn.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lto.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://oae.c1oappe.top

[E07] 按分隔符拆分
来源：http://cxs.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vvn.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lcs.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxi.ppjwa.cn

TS:   s.split(",")
来源：http://pqj.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://npx.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dzv.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://nnt.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uip.yonumen.top

[E08] 数组按分隔符合并
来源：http://otd.xuetiantiany.cn

Py:   ",".join(items)
来源：http://kow.fehbvm.com

PHP:  implode(",", $items);
来源：http://cgz.zhiwuduotai.top

JS:   items.join(",")
来源：http://otq.quarkkingdee.top

TS:   items.join(",")
来源：http://atd.xziqi.cn

Java: String.join(",", items)
来源：http://ujm.cashguo.top

Go:   strings.Join(items, ",")
来源：http://ynh.ctjpmb.com

Ruby: items.join(",")
来源：http://sps.gogol.net.cn

C#:   string.Join(",", items)
来源：http://ozn.guowangkeji.top

[E09] 去除所有空白字符
来源：http://vwx.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uob.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kvi.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://rop.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://unp.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://vzb.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://btg.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://rqk.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://okx.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://azz.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wwj.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cyd.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://ize.c1oappe.top


<!-- 参考信息 -->