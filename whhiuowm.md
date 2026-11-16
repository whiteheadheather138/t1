代发 wailian999

[D03] 在指定位置插入元素
来源：http://dks.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://vpy.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xqj.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lft.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://yxx.yj202588.top

Java: list.add(0, 0);
来源：http://fwk.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nwt.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pis.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://wph.sxryk.cn

[D04] 删除元素
来源：http://roo.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kck.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zke.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://upd.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://tkk.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wsd.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://khs.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ikq.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xac.haohaochexian.top

[D05] 访问与修改元素
来源：http://mym.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iga.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ezp.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nbt.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jyw.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://lsu.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://pco.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bee.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jar.bbcook.cn

[D06] 数组长度
来源：http://yjx.yj202588.top

Py:   len(arr)
来源：http://ans.cashguo.top

PHP:  count($arr);
来源：http://paz.zhongyouzk.top

JS:   arr.length
来源：http://ktv.zhoulong.xyz

TS:   arr.length
来源：http://ocj.ehwqpu.com

Java: list.size();
来源：http://ikr.yfazqb.com

Go:   len(arr)
来源：http://khr.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://sly.yuxming.cn

C#:   list.Count;
来源：http://nvx.hcnkem.com

[D07] 切片 / 取子数组
来源：http://jia.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://exu.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hbe.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://hmf.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://saj.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://agr.snrcjt.cn

Go:   arr[1:4]
来源：http://hnv.xziqi.cn

Ruby: arr[1, 3]
来源：http://pcq.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://zdx.hongshengwenyu.top

[D08] 合并两个数组
来源：http://usl.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://fjt.tanke756.top

PHP:  array_merge($a, $b);
来源：http://xfy.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nir.fzhhl.top

TS:   [...a, ...b];
来源：http://jvb.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smj.bbcook.cn

Go:   append(a, b...)
来源：http://vwg.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://yzt.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://ndf.ydjk.org.cn

[D09] 排序（升序）
来源：http://kxp.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://cqd.hnxiangtu.top

PHP:  sort($arr);
来源：http://drt.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://siz.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fcc.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://wnl.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fne.yj20258888.top

Ruby: arr.sort
来源：http://nyk.vqdsnc.cn

C#:   list.Sort();
来源：http://axp.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqn.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fjn.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://koc.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mec.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pys.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jnl.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xfq.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://odq.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ccr.smart0.xyz

[D11] 反转数组
来源：http://qxb.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://phh.epnwcf.com

PHP:  array_reverse($arr);
来源：http://dgx.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wkm.dianchejie.cn

TS:   [...arr].reverse();
来源：http://zpv.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://pbu.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://hqm.xinyue.icu

Ruby: arr.reverse
来源：http://oux.aibaodan.cn

C#:   list.Reverse();
来源：http://bkt.zhoulong.xyz

[D12] 查找元素下标
来源：http://ere.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://rjo.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jqt.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iku.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vum.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fei.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://wrw.sjlbkw.cn

Ruby: arr.index(x)
来源：http://syo.52xcode.cn

C#:   list.IndexOf(x);
来源：http://fey.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://ovz.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ieu.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dtt.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://dfx.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://zwz.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://onm.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nob.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://dsd.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ejw.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://dyh.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uaz.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tzp.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://ztp.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://vqw.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://myx.meibo888.top

Go:   // 手写循环
来源：http://gtv.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://win.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aqp.jinyuanbaomall.cn

[D15] 去重
来源：http://fck.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mzu.hammf.cn

PHP:  array_unique($arr);
来源：http://edv.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://zbd.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://ksj.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ohn.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ujs.zdqjudy.top

Ruby: arr.uniq
来源：http://nje.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://suz.xziqi.cn

[D16] 求和与平均值
来源：http://rph.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pch.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ieg.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpm.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dyl.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sbo.fehbvm.com

Go:   // 手写循环累加
来源：http://ouu.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rdy.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://oxt.gzhubu.top

[D17] 最大值与最小值
来源：http://knl.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://jjk.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://xeg.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ugq.sysykeji.top

TS:   Math.max(...arr);
来源：http://ohj.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gjn.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://umo.ivvv.top

Ruby: arr.max;  arr.min
来源：http://gea.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://tkp.cashguo.top

[D18] 扁平化嵌套数组
来源：http://pjy.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oli.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://xxj.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vbj.yongpay.top

TS:   nested.flat();
来源：http://dhg.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uid.hnxiangtu.top

Go:   // 手写双层循环
来源：http://ufb.dianchejie.cn

Ruby: nested.flatten
来源：http://xda.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cmk.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://aaj.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qba.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vfo.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kja.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dyo.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://enu.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://inc.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yzh.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ixp.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://foz.uphjek.com

Py:   Counter(arr)
来源：http://jrz.yvedp.cn

PHP:  array_count_values($arr);
来源：http://vaz.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ius.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbu.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jwi.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://vae.cqqwz.cn

Ruby: arr.tally
来源：http://xmb.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://plo.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://kyq.chenzaomai.com

Py:   x in arr
来源：http://mjl.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://hnb.ydzc1.top

JS:   arr.includes(x)
来源：http://qpi.daxiang520.top

TS:   arr.includes(x)
来源：http://api.feifeiyinyue.top

Java: list.contains(x)
来源：http://mle.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://nzu.ctjpmb.com

Ruby: arr.include?(x)
来源：http://csp.zhongyouzk.top

C#:   list.Contains(x)
来源：http://xnw.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://vmd.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eai.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jpf.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bct.wangdashe.top

TS:   [...arr];
来源：http://gjf.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://njq.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://udx.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://nkk.gzhubu.top

C#:   new List<int>(list);
来源：http://svd.jqgufenzy.top

[D23] reduce 累积计算
来源：http://fpv.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bqx.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fas.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qcv.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zkw.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ggh.shanyushiyangtech.top

Go:   // 手写循环
来源：http://rpj.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sjz.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sge.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://egk.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjd.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ufh.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bsc.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dmo.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tdg.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wyj.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uxb.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uhf.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://ogs.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jef.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://szr.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oys.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dbl.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lde.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tmy.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fuz.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vbx.gogol.net.cn

[D26] 数组转字符串
来源：http://rhb.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://oto.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://mbm.zycfv.cn

JS:   arr.join(", ")
来源：http://ryh.jianghu66.top

TS:   arr.join(", ")
来源：http://sjy.zhongyouzk.top

Java: String.join(", ", list)
来源：http://sry.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://jis.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://fhk.xziqi.cn

C#:   string.Join(", ", list)
来源：http://dkv.yuanzhike.top

================================================================================
来源：http://frc.zhaomingkeji.xyz

E. 字符串处理
来源：http://nlt.xuanzx.com

================================================================================
来源：http://dpl.yonumen.top

[E01] 拼接字符串
来源：http://sql.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nzt.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aot.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbn.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://htp.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rfd.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dzw.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fgq.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pbk.pycfn.com

[E02] 重复字符串
来源：http://lwk.kuanghao11.cn

Py:   "ab" * 3
来源：http://hcs.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://dkj.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://fio.gzhubu.top

TS:   "ab".repeat(3)
来源：http://gld.yuxming.cn

Java: "ab".repeat(3)
来源：http://nke.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://hhz.shzxlz.cn

Ruby: "ab" * 3
来源：http://lsf.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hfm.ybcxt.top

[E03] 截取子串
来源：http://jfj.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uot.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwt.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lar.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://rzd.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://ijp.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://amd.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://rgb.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://btl.hfpthk.cn

[E04] 查找子串位置
来源：http://lqg.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://vlx.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://kpr.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bjq.gzhubu.top

TS:   s.indexOf("x")
来源：http://bil.sweek.top

Java: s.indexOf("x")
来源：http://tcv.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://bmp.ctjpmb.com

Ruby: s.index("x")
来源：http://wkh.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://pmn.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://flp.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vdc.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kxh.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kik.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rbn.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xsa.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bgh.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zua.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tum.jlsjyb.cn

[E06] 替换子串
来源：http://jcl.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qac.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://hoj.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jui.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://vhe.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://abw.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://czv.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eri.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://icd.c1oappe.top

[E07] 按分隔符拆分
来源：http://ppo.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iub.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://edo.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cxv.nwbrower.top

TS:   s.split(",")
来源：http://sfh.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://skm.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ajm.yonumen.top

Ruby: s.split(",");  s.split
来源：http://bym.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hjx.52xcode.cn

[E08] 数组按分隔符合并
来源：http://nec.birdmap.top

Py:   ",".join(items)
来源：http://nag.hammf.cn

PHP:  implode(",", $items);
来源：http://hxj.snrcjt.cn

JS:   items.join(",")
来源：http://xvc.snrcjt.cn

TS:   items.join(",")
来源：http://scw.svipenyu.cn

Java: String.join(",", items)
来源：http://shk.316326.xyz

Go:   strings.Join(items, ",")
来源：http://vqf.hcnkem.com

Ruby: items.join(",")
来源：http://erx.pycfn.com

C#:   string.Join(",", items)
来源：http://kzp.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://fki.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gce.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eoi.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://jmo.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://dwx.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://ini.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bkh.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://gms.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://trg.52xcode.cn


<!-- 参考信息 -->