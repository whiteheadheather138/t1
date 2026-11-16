代发 wailian999

D. 数组 / 列表 / 集合
来源：http://jfr.0kj1m.cn

================================================================================
来源：http://zct.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://qae.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dhu.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://byb.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sys.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ank.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgn.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://bes.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://oug.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eoz.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://lyr.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nch.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vpl.hnxiangtu.top

JS:   arr.push(4);
来源：http://cyw.yongpay.top

TS:   arr.push(4);
来源：http://jet.jinyuanbaomall.cn

Java: list.add(4);
来源：http://qlt.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://cgz.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://igr.yvedp.cn

C#:   list.Add(4);
来源：http://pxd.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://ngu.yonumen.top

Py:   arr.insert(0, 0)
来源：http://tjv.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tef.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ehj.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://kmv.zdbjq.cn

Java: list.add(0, 0);
来源：http://ohs.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://oqe.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqr.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://xdj.fzhhl.top

[D04] 删除元素
来源：http://axs.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wui.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tys.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ven.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://saj.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xuh.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fjm.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rcd.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wsi.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://lkv.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://srd.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hez.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jqa.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://eag.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://nbf.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://nzj.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qlc.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jgd.mhx1999.top

[D06] 数组长度
来源：http://qvv.zhoulong.xyz

Py:   len(arr)
来源：http://gpm.yangfankeji.com

PHP:  count($arr);
来源：http://qhi.zhongyouzk.top

JS:   arr.length
来源：http://gee.xylfe.cn

TS:   arr.length
来源：http://dij.zycfv.cn

Java: list.size();
来源：http://cfp.ybcxt.top

Go:   len(arr)
来源：http://kbs.cucudq.cn

Ruby: arr.length; arr.size
来源：http://gno.fehbvm.com

C#:   list.Count;
来源：http://nss.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://ipc.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wlc.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://ntj.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://lfr.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://rfh.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://mub.hcnkem.com

Go:   arr[1:4]
来源：http://iud.ehwqpu.com

Ruby: arr[1, 3]
来源：http://hbk.jiagoushi.top

C#:   list.GetRange(1, 3);
来源：http://dje.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://mhm.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://kjw.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://qcf.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://azt.hnxiangtu.top

TS:   [...a, ...b];
来源：http://owr.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://keb.bjfxy.top

Go:   append(a, b...)
来源：http://mlg.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://bit.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://fir.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://pih.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://wvy.cucudq.cn

PHP:  sort($arr);
来源：http://qsh.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhk.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ced.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dis.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lcc.iojbl.cn

Ruby: arr.sort
来源：http://fkf.jinqigufen.top

C#:   list.Sort();
来源：http://aao.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xqz.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://khd.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xub.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bmk.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbn.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bcp.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zfu.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gsm.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ftw.shanyushiyangkeji.top

[D11] 反转数组
来源：http://xsd.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://ntx.yuxming.cn

PHP:  array_reverse($arr);
来源：http://vpq.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rnx.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://kns.nwbrower.top

Java: Collections.reverse(list);
来源：http://jje.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://hav.yuxming.cn

Ruby: arr.reverse
来源：http://kni.fzhhl.top

C#:   list.Reverse();
来源：http://zwo.guannengcc.top

[D12] 查找元素下标
来源：http://hrs.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://tdm.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://elf.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxl.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ftl.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qsb.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://pcb.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://oxz.yuxming.cn

C#:   list.IndexOf(x);
来源：http://pcw.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://rfg.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sfi.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yyr.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://nbk.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://jcb.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nep.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bdb.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ked.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hhb.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://rtu.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mvn.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qct.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://img.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://aoz.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://nbz.shzxlz.cn

Go:   // 手写循环
来源：http://pif.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lye.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pip.chenlongwang.top

[D15] 去重
来源：http://rxq.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sby.haohaochexian.top

PHP:  array_unique($arr);
来源：http://bft.fktsv.cn

JS:   [...new Set(arr)]
来源：http://jxr.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://lqu.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wmw.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vjn.aibaodan.cn

Ruby: arr.uniq
来源：http://rlg.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://pat.tianlin.xyz

[D16] 求和与平均值
来源：http://dcw.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://twi.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qww.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryw.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsy.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iso.snrcjt.cn

Go:   // 手写循环累加
来源：http://gvi.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ree.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://nqt.xinyue.icu

[D17] 最大值与最小值
来源：http://way.uphjek.com

Py:   max(arr);  min(arr)
来源：http://qgf.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://zxq.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dre.hywenlv.cn

TS:   Math.max(...arr);
来源：http://boj.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://sji.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kvg.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://ucw.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://rvi.sweek.top

[D18] 扁平化嵌套数组
来源：http://tap.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ewt.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://qhs.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kxo.dashuyun.cn

TS:   nested.flat();
来源：http://ewm.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://otm.hammf.cn

Go:   // 手写双层循环
来源：http://xpw.hongshengwenyu.top

Ruby: nested.flatten
来源：http://pnd.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zbs.yueranfly.top

[D19] 按字段分组
来源：http://zml.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ccn.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://phh.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rhr.tianlin.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://kgk.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zil.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://wif.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qjo.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pap.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://poo.jlsjyb.cn

Py:   Counter(arr)
来源：http://mrw.hnqzz.top

PHP:  array_count_values($arr);
来源：http://yqj.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ikc.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jvy.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bds.yj20258888.top

Go:   // 手写 map[T]int
来源：http://kqp.pycfn.com

Ruby: arr.tally
来源：http://fzo.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pev.xinyue.icu

[D21] 判断是否包含某元素
来源：http://ovk.yj202588.top

Py:   x in arr
来源：http://hen.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://rpx.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://lcu.hammf.cn

TS:   arr.includes(x)
来源：http://pjx.uphjek.com

Java: list.contains(x)
来源：http://wvz.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://cum.jiagoushi.top

Ruby: arr.include?(x)
来源：http://pyx.vehdjk.com

C#:   list.Contains(x)
来源：http://uop.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://cdy.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eyx.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjj.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qbe.52xcode.cn

TS:   [...arr];
来源：http://mow.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://ltu.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://pmb.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://vup.yvedp.cn

C#:   new List<int>(list);
来源：http://kdd.tarul.cn

[D23] reduce 累积计算
来源：http://uzc.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wwz.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jzr.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sal.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fiv.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nrp.vehdjk.com

Go:   // 手写循环
来源：http://wtv.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nfj.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvf.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://myg.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rxj.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aae.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bse.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jgy.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eiy.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kjg.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aze.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvv.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://kpe.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tax.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://err.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uyu.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kft.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pkm.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://saf.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://htc.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qjo.fengsongda.top

[D26] 数组转字符串
来源：http://ssh.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://teg.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://bro.vqdsnc.cn

JS:   arr.join(", ")
来源：http://ovt.sysykeji.top

TS:   arr.join(", ")
来源：http://cpc.chenjidiqi.icu

Java: String.join(", ", list)
来源：http://emj.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://kbn.cqqwz.cn

Ruby: arr.join(", ")
来源：http://lth.hammf.cn

C#:   string.Join(", ", list)
来源：http://vaw.jinyuanbaomall.cn

================================================================================
来源：http://fbg.shzxlz.cn

E. 字符串处理
来源：http://rbp.yuanzhike.top

================================================================================
来源：http://nbq.iojbl.cn

[E01] 拼接字符串
来源：http://ypq.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wjx.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rqj.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xht.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnt.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wql.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kuk.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jsh.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ymi.hysaishi.cn

[E02] 重复字符串
来源：http://niw.ctjpmb.com

Py:   "ab" * 3
来源：http://htn.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://xln.sweek.top

JS:   "ab".repeat(3)
来源：http://bsz.yj20258.top

TS:   "ab".repeat(3)
来源：http://jlt.andypj.xyz

Java: "ab".repeat(3)
来源：http://get.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://tht.hnqzz.top

Ruby: "ab" * 3
来源：http://xun.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ygk.tianlin.xyz

[E03] 截取子串
来源：http://hgr.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nva.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mvj.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wjb.xziqi.cn

TS:   s.slice(1, 4)
来源：http://pwd.c1oappe.top

Java: s.substring(1, 4)
来源：http://ruh.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fim.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://fnr.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://bty.ppjwa.cn

[E04] 查找子串位置
来源：http://lsi.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://xgb.tarul.cn

PHP:  strpos($s, "x");
来源：http://oit.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rxk.svipenyu.cn

TS:   s.indexOf("x")
来源：http://kny.9152youxi.cn

Java: s.indexOf("x")
来源：http://jge.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://cxj.yvedp.cn

Ruby: s.index("x")
来源：http://qom.hcnkem.com

C#:   s.IndexOf("x")
来源：http://ogy.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ysi.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hwe.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jsw.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igp.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fmz.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ymd.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mzq.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lik.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xut.dianchejie.cn

[E06] 替换子串
来源：http://sqk.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gjp.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://bng.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://itg.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://cay.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnu.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gow.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jkt.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://sji.yangfankeji.com

[E07] 按分隔符拆分
来源：http://sxr.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zib.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nrd.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ybo.havefunace.top

TS:   s.split(",")
来源：http://uwf.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sov.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ytn.meibo888.top


<!-- 参考信息 -->