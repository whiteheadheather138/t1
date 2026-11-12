代发 wailian999

PHP:  // 无重载
来源：http://dcs.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wfh.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://lnt.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xhf.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://axf.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://zmn.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sbv.gotoacloud.top

================================================================================
来源：http://wdc.hammf.cn

D. 数组 / 列表 / 集合
来源：http://ojc.hammf.cn

================================================================================
来源：http://tvi.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://ljj.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rmx.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cby.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iwn.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://fwu.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://caa.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://fvq.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://rck.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lkr.redwolf501.top

[D02] 追加元素到末尾
来源：http://pjc.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ifi.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zcn.ydjk.org.cn

JS:   arr.push(4);
来源：http://yfz.cheryme.top

TS:   arr.push(4);
来源：http://pjf.yanxiufei.cn

Java: list.add(4);
来源：http://lma.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://zxr.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://ump.hywenlv.cn

C#:   list.Add(4);
来源：http://ojb.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://aub.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://umr.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://awr.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lgc.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://ksm.zhoulong.xyz

Java: list.add(0, 0);
来源：http://vze.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tvp.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://osz.cheryme.top

C#:   list.Insert(0, 0);
来源：http://xsw.daria6918.cn

[D04] 删除元素
来源：http://sen.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jyc.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwk.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cbc.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://knv.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://igq.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fth.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fiz.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cpd.vqdsnc.cn

[D05] 访问与修改元素
来源：http://nst.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ias.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ulk.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vck.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://kni.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://wmf.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://aci.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jrx.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xep.cqqwz.cn

[D06] 数组长度
来源：http://uhd.shzxlz.cn

Py:   len(arr)
来源：http://ysh.yj202588.top

PHP:  count($arr);
来源：http://vvw.kuanghao11.cn

JS:   arr.length
来源：http://uan.fanxiaobao.xyz

TS:   arr.length
来源：http://uuk.dashuyun.cn

Java: list.size();
来源：http://hiw.bjfxy.top

Go:   len(arr)
来源：http://rwm.birdmap.top

Ruby: arr.length; arr.size
来源：http://wok.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://tbr.yuxming.cn

[D07] 切片 / 取子数组
来源：http://rkv.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qzn.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://oqi.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://qhn.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://qfa.cucudq.cn

Java: list.subList(1, 4);
来源：http://fhx.xylfe.cn

Go:   arr[1:4]
来源：http://blo.snrcjt.cn

Ruby: arr[1, 3]
来源：http://xhc.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://ubj.andypj.xyz

[D08] 合并两个数组
来源：http://fnr.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://urz.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://dli.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eco.meibo888.top

TS:   [...a, ...b];
来源：http://htp.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://njx.uphjek.com

Go:   append(a, b...)
来源：http://gfj.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://ich.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://rux.quarkkingdee.top

[D09] 排序（升序）
来源：http://kvl.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://hwf.epnwcf.com

PHP:  sort($arr);
来源：http://jlz.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzh.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sjg.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nau.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jnr.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://kam.meibo888.top

C#:   list.Sort();
来源：http://neb.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gip.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ocr.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhy.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://plh.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzh.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gft.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lks.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tgr.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nmf.hnxiangtu.top

[D11] 反转数组
来源：http://xid.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zpf.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://ykg.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ban.yuxming.cn

TS:   [...arr].reverse();
来源：http://mog.yangfankeji.com

Java: Collections.reverse(list);
来源：http://hui.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://tiz.kuanghao11.cn

Ruby: arr.reverse
来源：http://six.zdbjq.cn

C#:   list.Reverse();
来源：http://qhm.ehwqpu.com

[D12] 查找元素下标
来源：http://loz.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://zox.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qep.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dnr.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmf.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vhj.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://iay.yonumen.top

Ruby: arr.index(x)
来源：http://jnl.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://xhf.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://gry.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://trb.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://apx.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://rik.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://zlc.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://afa.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://esx.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://okx.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://win.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://ppr.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hpx.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vnd.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://bqz.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://paq.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ihx.chenlongwang.top

Go:   // 手写循环
来源：http://zjl.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://yzh.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nxr.hywenlv.cn

[D15] 去重
来源：http://eqb.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pxl.tianlin.xyz

PHP:  array_unique($arr);
来源：http://dzq.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://vnh.daria6918.cn

TS:   [...new Set(arr)]
来源：http://hru.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qtw.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://vzy.yanxiufei.cn

Ruby: arr.uniq
来源：http://mag.sweek.top

C#:   list.Distinct().ToList()
来源：http://qlh.yuxming.cn

[D16] 求和与平均值
来源：http://wbe.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ppp.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://swv.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vie.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjc.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://edd.svipenyu.cn

Go:   // 手写循环累加
来源：http://htq.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bqf.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://cky.yvedp.cn

[D17] 最大值与最小值
来源：http://zht.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://mgl.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://chi.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ksj.xylfe.cn

TS:   Math.max(...arr);
来源：http://djj.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iuq.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wvz.tanke756.top

Ruby: arr.max;  arr.min
来源：http://beo.cashguo.top

C#:   list.Max();  list.Min()
来源：http://pvx.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://fhz.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eiv.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://xca.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://snc.xinyue.icu

TS:   nested.flat();
来源：http://ncw.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mmq.nanxinkj.top

Go:   // 手写双层循环
来源：http://rla.gaohongyu789.top

Ruby: nested.flatten
来源：http://kmo.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://oog.jyoumei.cn

[D19] 按字段分组
来源：http://emu.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nnz.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xuw.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jgc.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://isz.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vga.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://ogw.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fug.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kco.sweek.top

[D20] 统计每个元素出现次数
来源：http://sbz.316326.xyz

Py:   Counter(arr)
来源：http://dmd.fehbvm.com

PHP:  array_count_values($arr);
来源：http://ayy.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqd.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvj.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ebn.meibo888.top

Go:   // 手写 map[T]int
来源：http://mva.zhoulong.xyz

Ruby: arr.tally
来源：http://eby.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dnx.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://qmd.shzxlz.cn

Py:   x in arr
来源：http://pqy.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://wlv.jinqigufen.top

JS:   arr.includes(x)
来源：http://sas.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://mpr.yuxming.cn

Java: list.contains(x)
来源：http://mgo.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://vik.shuidangran.top

Ruby: arr.include?(x)
来源：http://omt.bjfxy.top

C#:   list.Contains(x)
来源：http://jag.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://jgj.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yyf.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oid.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vjr.jqgufenzy.top

TS:   [...arr];
来源：http://kwo.daxiang520.top

Java: new ArrayList<>(list);
来源：http://rch.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://svs.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://fiz.52xcode.cn

C#:   new List<int>(list);
来源：http://pqj.ydzc1.top

[D23] reduce 累积计算
来源：http://bgd.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgf.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qnn.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exb.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tkr.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bfo.tarul.cn

Go:   // 手写循环
来源：http://wbe.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lko.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wrv.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://jtv.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://leb.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yte.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dzm.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nyj.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ssf.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ugc.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aot.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvt.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://rom.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xwk.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hzo.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aoe.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ewg.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dth.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wbs.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xdh.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hyq.guowangkeji.top

[D26] 数组转字符串
来源：http://knv.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://kcd.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://cya.nanxuanxn.top

JS:   arr.join(", ")
来源：http://dhl.52xcode.cn

TS:   arr.join(", ")
来源：http://zlt.tian-w.cn

Java: String.join(", ", list)
来源：http://xqf.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://fcp.ctjpmb.com

Ruby: arr.join(", ")
来源：http://gbg.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://uoz.vehdjk.com

================================================================================
来源：http://aib.shanyushiyangtech.top

E. 字符串处理
来源：http://fmj.tianlin.xyz

================================================================================
来源：http://iib.zycfv.cn

[E01] 拼接字符串
来源：http://oop.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jzq.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ydf.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eoj.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbd.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://flz.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdc.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dah.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yfu.fktsv.cn

[E02] 重复字符串
来源：http://iox.c1oappe.top

Py:   "ab" * 3
来源：http://jzn.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://foy.wangdashe.top

JS:   "ab".repeat(3)
来源：http://nup.cucudq.cn

TS:   "ab".repeat(3)
来源：http://thy.snrcjt.cn

Java: "ab".repeat(3)
来源：http://lgy.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://drg.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://dbu.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://res.hywenlv.cn

[E03] 截取子串
来源：http://oko.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://saq.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://avl.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ege.nwbrower.top

TS:   s.slice(1, 4)
来源：http://fcp.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://gfm.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pvt.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://lhb.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://yxf.guowangkeji.top

[E04] 查找子串位置
来源：http://oyn.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://tps.52xcode.cn

PHP:  strpos($s, "x");
来源：http://gqo.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://poh.gzhubu.top

TS:   s.indexOf("x")
来源：http://wjg.sjlbkw.cn

Java: s.indexOf("x")
来源：http://xdb.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://zkf.kuanghao11.cn

Ruby: s.index("x")
来源：http://hbn.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://rjp.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ohu.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ngm.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqd.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://okj.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://asg.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zkn.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dal.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://way.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jom.yuxming.cn

[E06] 替换子串
来源：http://mqo.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yzr.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://zhz.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ycw.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://fjt.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyr.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rfm.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vzj.jqgfzy.top


<!-- 参考信息 -->