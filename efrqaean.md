代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oiv.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wii.hcnkem.com

JS:   arr.push(4);
来源：http://nky.bjfxy.top

TS:   arr.push(4);
来源：http://rry.ybcxt.top

Java: list.add(4);
来源：http://cvo.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://ptu.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://ifs.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://dbn.fehbvm.com

[D03] 在指定位置插入元素
来源：http://piu.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://zlr.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tdx.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cxi.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://hcw.fengsongda.top

Java: list.add(0, 0);
来源：http://ork.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fll.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zmz.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://osd.zdbjq.cn

[D04] 删除元素
来源：http://chu.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iad.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tmk.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wes.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://fup.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jhc.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yfa.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cer.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pon.yongpay.top

[D05] 访问与修改元素
来源：http://cch.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://grh.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oxl.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ugy.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://gqo.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://amq.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://wrl.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://acg.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fmz.wangdashe.top

[D06] 数组长度
来源：http://nvw.tarul.cn

Py:   len(arr)
来源：http://qdb.aibaodan.cn

PHP:  count($arr);
来源：http://zov.fanxiaobao.xyz

JS:   arr.length
来源：http://tot.c1oappe.top

TS:   arr.length
来源：http://ykm.svipenyu.cn

Java: list.size();
来源：http://ppt.cashguo.top

Go:   len(arr)
来源：http://hyp.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://fhw.jinyuanbaomall.cn

C#:   list.Count;
来源：http://ixr.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://jzi.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ygr.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vag.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://ten.tanke756.top

TS:   arr.slice(1, 4);
来源：http://oim.fehbvm.com

Java: list.subList(1, 4);
来源：http://pas.shzxlz.cn

Go:   arr[1:4]
来源：http://atb.ivvv.top

Ruby: arr[1, 3]
来源：http://osl.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://mau.aibaodan.cn

[D08] 合并两个数组
来源：http://ihe.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://tny.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://qgn.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qgf.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://kff.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgo.hnqzz.top

Go:   append(a, b...)
来源：http://jiz.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://ovt.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://ero.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://ysj.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://agu.tanke756.top

PHP:  sort($arr);
来源：http://soe.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mvr.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://umu.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zgy.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nsh.tarul.cn

Ruby: arr.sort
来源：http://vlu.hcnkem.com

C#:   list.Sort();
来源：http://eux.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://orf.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jmw.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://miw.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fcj.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eda.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ydc.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lxi.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jnl.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zzy.xziqi.cn

[D11] 反转数组
来源：http://hen.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cux.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://wto.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kyl.yfazqb.com

TS:   [...arr].reverse();
来源：http://lby.fehbvm.com

Java: Collections.reverse(list);
来源：http://mle.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://zoa.xylfe.cn

Ruby: arr.reverse
来源：http://tuo.meibo888.top

C#:   list.Reverse();
来源：http://puy.daxiang520.top

[D12] 查找元素下标
来源：http://eqc.sweek.top

Py:   arr.index(x);  x in arr
来源：http://fyf.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nha.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyk.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pzr.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://koq.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://zce.andypj.xyz

Ruby: arr.index(x)
来源：http://xca.ivvv.top

C#:   list.IndexOf(x);
来源：http://ium.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://vho.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://col.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nzi.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://tpe.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://kjl.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kte.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jrw.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cfs.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ktf.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://pqc.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rfg.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nmu.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://xwi.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://btb.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ivx.andypj.xyz

Go:   // 手写循环
来源：http://kdb.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uwp.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://twc.snrcjt.cn

[D15] 去重
来源：http://eof.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mza.cheryme.top

PHP:  array_unique($arr);
来源：http://ptt.vehdjk.com

JS:   [...new Set(arr)]
来源：http://lit.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://xvu.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mxl.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://eua.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://opr.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://zkh.zhongyouzk.top

[D16] 求和与平均值
来源：http://ero.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hdn.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gaz.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsj.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifb.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqe.shuidangran.top

Go:   // 手写循环累加
来源：http://dfw.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bsb.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://prq.smart0.xyz

[D17] 最大值与最小值
来源：http://ydx.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://jal.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://oeu.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yez.chenzaomai.com

TS:   Math.max(...arr);
来源：http://jfn.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xbh.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hlt.uphjek.com

Ruby: arr.max;  arr.min
来源：http://npj.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://idv.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://aqq.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://exl.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://erc.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hxj.yonumen.top

TS:   nested.flat();
来源：http://hjm.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ytc.guannengcc.top

Go:   // 手写双层循环
来源：http://vts.zycfv.cn

Ruby: nested.flatten
来源：http://nok.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://brx.tianlin.xyz

[D19] 按字段分组
来源：http://lcz.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://svp.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yau.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rsc.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xix.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nhp.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://qsq.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fka.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yve.birdmap.top

[D20] 统计每个元素出现次数
来源：http://vxc.ctjpmb.com

Py:   Counter(arr)
来源：http://uyc.ybcxt.top

PHP:  array_count_values($arr);
来源：http://hwf.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqv.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nar.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ihe.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://smk.sjlbkw.cn

Ruby: arr.tally
来源：http://orl.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://akd.yvedp.cn

[D21] 判断是否包含某元素
来源：http://uti.chenzaomai.com

Py:   x in arr
来源：http://boj.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://adl.vehdjk.com

JS:   arr.includes(x)
来源：http://prv.epnwcf.com

TS:   arr.includes(x)
来源：http://xgu.xuanzx.com

Java: list.contains(x)
来源：http://goj.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://mmb.vehdjk.com

Ruby: arr.include?(x)
来源：http://xri.sxryk.cn

C#:   list.Contains(x)
来源：http://jmp.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://oij.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trb.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tse.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hos.vqdsnc.cn

TS:   [...arr];
来源：http://mmj.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://hzs.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://fjx.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://ktj.ybcxt.top

C#:   new List<int>(list);
来源：http://gyi.uphjek.com

[D23] reduce 累积计算
来源：http://fyk.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gnl.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmw.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nra.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ior.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ukd.tianlin.xyz

Go:   // 手写循环
来源：http://mag.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gxn.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qgv.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://bhx.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dbk.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tzw.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oux.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wrm.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ceb.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://agx.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nub.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xme.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://ggh.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bzx.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gzv.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bug.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wmu.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jza.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dnj.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xkv.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xwa.hnqzz.top

[D26] 数组转字符串
来源：http://trb.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://jgn.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://uya.havefunace.top

JS:   arr.join(", ")
来源：http://bgr.yfazqb.com

TS:   arr.join(", ")
来源：http://hug.ppjwa.cn

Java: String.join(", ", list)
来源：http://dfi.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://gls.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://vpo.jianghu66.top

C#:   string.Join(", ", list)
来源：http://jzg.zycfv.cn

================================================================================
来源：http://uzj.yongpay.top

E. 字符串处理
来源：http://nln.jlsjyb.cn

================================================================================
来源：http://fgz.gzhubu.top

[E01] 拼接字符串
来源：http://wax.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vzl.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tcl.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qca.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qou.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yxx.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rpd.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eoc.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xvb.cucudq.cn

[E02] 重复字符串
来源：http://bja.ydzc1.top

Py:   "ab" * 3
来源：http://vaq.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://snl.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://cpq.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://pen.snrcjt.cn

Java: "ab".repeat(3)
来源：http://iog.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://jev.epnwcf.com

Ruby: "ab" * 3
来源：http://xgs.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rcu.aizwys.cn

[E03] 截取子串
来源：http://rgo.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jiz.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vjw.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nub.daria6918.cn

TS:   s.slice(1, 4)
来源：http://zod.52xcode.cn

Java: s.substring(1, 4)
来源：http://mbg.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tpw.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bsn.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://wuy.vqdsnc.cn

[E04] 查找子串位置
来源：http://nbf.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://zep.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://mar.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zqn.meibo888.top

TS:   s.indexOf("x")
来源：http://ayw.c1oappe.top

Java: s.indexOf("x")
来源：http://lgr.316326.xyz

Go:   strings.Index(s, "x")
来源：http://ogd.yj20258888.top

Ruby: s.index("x")
来源：http://eug.yvedp.cn

C#:   s.IndexOf("x")
来源：http://efv.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://veb.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vnk.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tyd.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cis.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qtp.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pwh.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://svo.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ods.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rjy.iojbl.cn

[E06] 替换子串
来源：http://tuw.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xiq.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://shc.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdl.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://fis.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zko.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://opx.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ktz.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://thf.redwolf501.top

[E07] 按分隔符拆分
来源：http://som.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iyl.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xbu.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pdq.vqdsnc.cn

TS:   s.split(",")
来源：http://mrd.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zch.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hmp.kuanghao11.cn

Ruby: s.split(",");  s.split
来源：http://dnh.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ysl.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://ykb.cucudq.cn

Py:   ",".join(items)
来源：http://aas.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://qlu.nanxuanxn.top

JS:   items.join(",")
来源：http://ewv.guannengcc.top

TS:   items.join(",")
来源：http://bup.guowangkeji.top

Java: String.join(",", items)
来源：http://moz.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://dsc.wangdashe.top

Ruby: items.join(",")
来源：http://ldg.hcnkem.com

C#:   string.Join(",", items)
来源：http://hpe.cdnleiting.top

[E09] 去除所有空白字符
来源：http://ifw.gaohongyu789.top


<!-- 参考信息 -->