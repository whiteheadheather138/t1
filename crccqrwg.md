代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://yqx.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://jja.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qfx.c1oappe.top

[D02] 追加元素到末尾
来源：http://pdk.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pfs.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ufj.chenzaomai.com

JS:   arr.push(4);
来源：http://osk.zdqjudy.top

TS:   arr.push(4);
来源：http://irr.yuanzhike.top

Java: list.add(4);
来源：http://kct.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://pcn.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://kxq.hcnkem.com

C#:   list.Add(4);
来源：http://vip.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://oai.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://rjr.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rid.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://znr.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://svw.0kj1m.cn

Java: list.add(0, 0);
来源：http://hay.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vnc.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fpg.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://fnu.zdbjq.cn

[D04] 删除元素
来源：http://dhk.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://meb.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xif.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tdn.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://lej.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wnd.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gnv.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fss.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tlt.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://bsa.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zgc.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://auw.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tlf.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://rgt.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://rth.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://xnq.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gul.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mfe.shangyingyoupin.top

[D06] 数组长度
来源：http://oll.jinqigfzy.top

Py:   len(arr)
来源：http://knx.shzxlz.cn

PHP:  count($arr);
来源：http://euz.zhijiandao.cn

JS:   arr.length
来源：http://qfy.xziqi.cn

TS:   arr.length
来源：http://fzx.gaohongyu789.top

Java: list.size();
来源：http://wne.yj20258.top

Go:   len(arr)
来源：http://lzd.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://iak.svipenyu.cn

C#:   list.Count;
来源：http://qbc.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://wyl.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://guw.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gin.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://wgv.meibo888.top

TS:   arr.slice(1, 4);
来源：http://wvx.shuidangran.top

Java: list.subList(1, 4);
来源：http://ohk.daria6918.cn

Go:   arr[1:4]
来源：http://shp.snrcjt.cn

Ruby: arr[1, 3]
来源：http://rdk.sweek.top

C#:   list.GetRange(1, 3);
来源：http://vut.andypj.xyz

[D08] 合并两个数组
来源：http://ezx.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://ixh.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://oes.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hlh.yj20258.top

TS:   [...a, ...b];
来源：http://icd.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://krs.gotoacloud.top

Go:   append(a, b...)
来源：http://zhv.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://fnl.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://qqj.zhixingplan.top

[D09] 排序（升序）
来源：http://ert.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://tks.fehbvm.com

PHP:  sort($arr);
来源：http://hdu.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aav.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mnm.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://esd.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ayk.cdnleiting.top

Ruby: arr.sort
来源：http://aza.fengsongda.top

C#:   list.Sort();
来源：http://ipq.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oas.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rmz.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whn.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxt.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wuz.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sfd.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nqk.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yvs.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tcd.aizwys.cn

[D11] 反转数组
来源：http://cik.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://pmc.meibo888.top

PHP:  array_reverse($arr);
来源：http://gtm.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmr.zdqjudy.top

TS:   [...arr].reverse();
来源：http://ten.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://qjg.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://ymd.yangfankeji.com

Ruby: arr.reverse
来源：http://ypu.aizwys.cn

C#:   list.Reverse();
来源：http://apw.tian-w.cn

[D12] 查找元素下标
来源：http://ozu.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://pva.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://afd.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pee.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yeg.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yyv.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://dsh.jyoumei.cn

Ruby: arr.index(x)
来源：http://mwq.redwolf501.top

C#:   list.IndexOf(x);
来源：http://ags.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://acv.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gdw.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hjl.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://xew.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://jzn.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gsy.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mgu.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://unp.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rrd.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://amh.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xve.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ygq.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://egw.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://zut.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gok.meibo888.top

Go:   // 手写循环
来源：http://cia.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://koj.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bcu.aibaodan.cn

[D15] 去重
来源：http://neq.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wol.tarul.cn

PHP:  array_unique($arr);
来源：http://gxr.redwolf501.top

JS:   [...new Set(arr)]
来源：http://fng.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://jwy.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://njz.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://riz.meibo888.top

Ruby: arr.uniq
来源：http://rsp.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://onw.jyoumei.cn

[D16] 求和与平均值
来源：http://mzk.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lta.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xss.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qdd.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eri.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://chd.zhijiandao.cn

Go:   // 手写循环累加
来源：http://wfi.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jub.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://hag.bjfxy.top

[D17] 最大值与最小值
来源：http://voq.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://xff.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://pyq.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://frl.fengsongda.top

TS:   Math.max(...arr);
来源：http://pgz.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jtv.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yha.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://chn.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://olv.uphjek.com

[D18] 扁平化嵌套数组
来源：http://zwg.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cdj.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://itp.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ucp.nanxinkj.top

TS:   nested.flat();
来源：http://axt.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kcd.shzxlz.cn

Go:   // 手写双层循环
来源：http://qdy.svipenyu.cn

Ruby: nested.flatten
来源：http://idz.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://txi.iojbl.cn

[D19] 按字段分组
来源：http://wor.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://der.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lfw.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hvg.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pfz.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jga.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://cqs.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gpm.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://icm.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://kfs.fehbvm.com

Py:   Counter(arr)
来源：http://fjl.havefunace.top

PHP:  array_count_values($arr);
来源：http://naf.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lif.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ewu.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpo.hesvh.cn

Go:   // 手写 map[T]int
来源：http://ppm.0kj1m.cn

Ruby: arr.tally
来源：http://vmz.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ukn.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://tjw.ydjk.org.cn

Py:   x in arr
来源：http://crf.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://qgk.cucudq.cn

JS:   arr.includes(x)
来源：http://qgz.tanke756.top

TS:   arr.includes(x)
来源：http://hay.jinghuilouyu.cn

Java: list.contains(x)
来源：http://wkj.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://bcb.zycfv.cn

Ruby: arr.include?(x)
来源：http://exc.uphjek.com

C#:   list.Contains(x)
来源：http://ito.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://bhw.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqb.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sct.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pcz.haohaochexian.top

TS:   [...arr];
来源：http://hea.yj20258.top

Java: new ArrayList<>(list);
来源：http://dhe.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://avu.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://otn.meibo888.top

C#:   new List<int>(list);
来源：http://kpr.nanxinkj.top

[D23] reduce 累积计算
来源：http://bkf.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rhk.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uky.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elx.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyn.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://pqo.aizwys.cn

Go:   // 手写循环
来源：http://fwm.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dmb.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://spp.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://hre.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mhg.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngl.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xea.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wbb.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbe.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zwa.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dnd.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wyq.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://jzg.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://otq.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sph.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://axs.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qjl.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oyx.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sfe.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cyc.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jxb.zdqjudy.top

[D26] 数组转字符串
来源：http://mmc.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://akk.sweek.top

PHP:  implode(", ", $arr);
来源：http://mwe.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://dux.chenlongwang.top

TS:   arr.join(", ")
来源：http://jqa.meibo888.top

Java: String.join(", ", list)
来源：http://dog.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://cse.sxryk.cn

Ruby: arr.join(", ")
来源：http://ynd.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://wou.shuidangran.top

================================================================================
来源：http://qin.gaohongyu789.top

E. 字符串处理
来源：http://ido.sysykeji.top

================================================================================
来源：http://ter.uphjek.com

[E01] 拼接字符串
来源：http://vri.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fwo.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fdh.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zbs.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvd.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nmt.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nhg.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xnn.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ubl.yonumen.top

[E02] 重复字符串
来源：http://ybz.sjlbkw.cn

Py:   "ab" * 3
来源：http://zhl.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://pji.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://cgs.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://kin.meibo888.top

Java: "ab".repeat(3)
来源：http://zgm.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://aly.jianghu66.top

Ruby: "ab" * 3
来源：http://gtr.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://muz.jinghuilouyu.cn

[E03] 截取子串
来源：http://cwb.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xcd.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sam.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jic.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://gvm.zdqjudy.top

Java: s.substring(1, 4)
来源：http://rtr.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://krl.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://ihe.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://kdy.fengsongda.top

[E04] 查找子串位置
来源：http://zfp.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://acs.daxiang520.top

PHP:  strpos($s, "x");
来源：http://qvm.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oij.yongpay.top

TS:   s.indexOf("x")
来源：http://eav.jiagoushi.top

Java: s.indexOf("x")
来源：http://ojg.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://rcl.snrcjt.cn

Ruby: s.index("x")
来源：http://nbt.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://zpd.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jhl.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vwc.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eod.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tfb.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oyy.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://siu.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qem.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://txu.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kkp.shangyingyoupin.top

[E06] 替换子串
来源：http://hlx.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ejs.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://uyf.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vrc.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://rfi.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwg.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://khi.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fym.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://sdh.yangfankeji.com

[E07] 按分隔符拆分
来源：http://lox.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://swz.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pyd.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wlu.9152youxi.cn

TS:   s.split(",")
来源：http://xbj.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://nqh.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nwe.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://htc.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qsx.nwbrower.top

[E08] 数组按分隔符合并
来源：http://lpp.chenzaomai.com

Py:   ",".join(items)
来源：http://iev.yueranfly.top

PHP:  implode(",", $items);
来源：http://jsp.jinqigfzy.top

JS:   items.join(",")
来源：http://kxw.hywenlv.cn

TS:   items.join(",")
来源：http://frw.dianchejie.cn

Java: String.join(",", items)
来源：http://xiq.cashguo.top


<!-- 参考信息 -->