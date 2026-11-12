代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://dbh.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://ans.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://akc.yuanzhike.top

[D02] 追加元素到末尾
来源：http://ofv.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iqc.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rrp.hongshengwenyu.top

JS:   arr.push(4);
来源：http://spe.cashguo.top

TS:   arr.push(4);
来源：http://vwj.ivvv.top

Java: list.add(4);
来源：http://vem.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://kyo.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://scf.snrcjt.cn

C#:   list.Add(4);
来源：http://glj.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://pph.yongpay.top

Py:   arr.insert(0, 0)
来源：http://yjg.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://msu.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wpu.ybcxt.top

TS:   arr.splice(0, 0, 0);
来源：http://eoz.yueranfly.top

Java: list.add(0, 0);
来源：http://bsc.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://hjt.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qby.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://qvt.shzxlz.cn

[D04] 删除元素
来源：http://gto.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://znc.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wyo.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zxu.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://lsw.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ntb.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tjq.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://abg.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://muh.c1oappe.top

[D05] 访问与修改元素
来源：http://hqx.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tod.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ulv.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ycm.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://tkr.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://xxb.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://qov.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ggk.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yti.c1oappe.top

[D06] 数组长度
来源：http://fpy.xziqi.cn

Py:   len(arr)
来源：http://xgl.xinyue.icu

PHP:  count($arr);
来源：http://jgl.meibo888.top

JS:   arr.length
来源：http://vvw.cucudq.cn

TS:   arr.length
来源：http://woe.yfazqb.com

Java: list.size();
来源：http://lai.bbcook.cn

Go:   len(arr)
来源：http://cac.havefunace.top

Ruby: arr.length; arr.size
来源：http://cyj.zdqjudy.top

C#:   list.Count;
来源：http://riu.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://kmw.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://woj.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rah.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://ztu.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://yrw.xinyue.icu

Java: list.subList(1, 4);
来源：http://bpk.zdqjudy.top

Go:   arr[1:4]
来源：http://wmb.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://isn.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://fgk.zhijiandao.cn

[D08] 合并两个数组
来源：http://krc.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://wnk.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://jph.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jjp.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://bbe.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ykf.pengpengdd.cyou

Go:   append(a, b...)
来源：http://hod.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://ogc.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://gbi.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://lmy.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://tvz.xuetiantiany.cn

PHP:  sort($arr);
来源：http://lcn.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ffp.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://doq.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uts.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://teq.jianghu66.top

Ruby: arr.sort
来源：http://ijf.mhx1999.top

C#:   list.Sort();
来源：http://eoz.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://dol.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tam.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dkm.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmc.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgr.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dbt.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://onb.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rtm.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gfe.ybcxt.top

[D11] 反转数组
来源：http://vzk.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://clg.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://upv.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qtj.yvedp.cn

TS:   [...arr].reverse();
来源：http://hvr.yvedp.cn

Java: Collections.reverse(list);
来源：http://gde.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://kdx.316326.xyz

Ruby: arr.reverse
来源：http://onm.yuxming.cn

C#:   list.Reverse();
来源：http://gdx.hywenlv.cn

[D12] 查找元素下标
来源：http://wnj.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://bdd.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lhe.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gos.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://diy.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baz.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://ayd.smart0.xyz

Ruby: arr.index(x)
来源：http://swq.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://lxr.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://ceg.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zdr.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jno.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://fhf.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://tjw.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ity.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cvh.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gle.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dai.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://rfs.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://efo.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ppg.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://xlg.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://jvw.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pss.yj20258888.top

Go:   // 手写循环
来源：http://fzt.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://kic.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qql.zdqjudy.top

[D15] 去重
来源：http://uid.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vgt.xuanzx.com

PHP:  array_unique($arr);
来源：http://xui.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://kle.yfazqb.com

TS:   [...new Set(arr)]
来源：http://rfz.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ijo.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://yyk.fzhhl.top

Ruby: arr.uniq
来源：http://jdn.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://sib.yj202588.top

[D16] 求和与平均值
来源：http://tjl.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://btf.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gvw.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pce.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzj.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hho.snrcjt.cn

Go:   // 手写循环累加
来源：http://cjh.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jke.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://lbx.gogol.net.cn

[D17] 最大值与最小值
来源：http://tcz.yj20258.top

Py:   max(arr);  min(arr)
来源：http://mod.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://jfh.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qut.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://yyu.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://spk.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ciy.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://zuo.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://ert.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://dvc.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ohm.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://pom.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wnc.guannengcc.top

TS:   nested.flat();
来源：http://gbs.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rep.316326.xyz

Go:   // 手写双层循环
来源：http://iij.shangyingyoupin.top

Ruby: nested.flatten
来源：http://itw.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lxs.yueranfly.top

[D19] 按字段分组
来源：http://pdw.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zpq.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pqk.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lis.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://udw.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jav.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://iof.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zat.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uas.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://avu.hysaishi.cn

Py:   Counter(arr)
来源：http://kua.vehdjk.com

PHP:  array_count_values($arr);
来源：http://fil.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tgn.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dnt.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lbp.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://azr.fzhhl.top

Ruby: arr.tally
来源：http://icb.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rik.sxryk.cn

[D21] 判断是否包含某元素
来源：http://log.mhx1999.top

Py:   x in arr
来源：http://kpr.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://vaa.aizwys.cn

JS:   arr.includes(x)
来源：http://kmw.zhoulong.xyz

TS:   arr.includes(x)
来源：http://ilj.cucudq.cn

Java: list.contains(x)
来源：http://cub.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://ptu.xylfe.cn

Ruby: arr.include?(x)
来源：http://kaf.tanke756.top

C#:   list.Contains(x)
来源：http://jil.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://dix.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://psg.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sjo.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uoq.cucudq.cn

TS:   [...arr];
来源：http://jex.xinyue.icu

Java: new ArrayList<>(list);
来源：http://cnu.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://xwi.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://cgf.redwolf501.top

C#:   new List<int>(list);
来源：http://biz.xziqi.cn

[D23] reduce 累积计算
来源：http://phh.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bbz.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uor.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tcy.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azd.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hww.yanxiufei.cn

Go:   // 手写循环
来源：http://hyb.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pso.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mic.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://vxf.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bsw.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://juk.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwv.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ork.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nzg.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qgh.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwv.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wok.birdmap.top

[D25] Set 集合去重与交并差
来源：http://yom.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oeo.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://adt.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gxs.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mmr.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://irs.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://akr.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dhy.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jlz.shzxlz.cn

[D26] 数组转字符串
来源：http://ept.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://nyw.uphjek.com

PHP:  implode(", ", $arr);
来源：http://htv.birdmap.top

JS:   arr.join(", ")
来源：http://mtz.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://orz.hnxiangtu.top

Java: String.join(", ", list)
来源：http://awp.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://slu.tianlin.xyz

Ruby: arr.join(", ")
来源：http://vfn.cashguo.top

C#:   string.Join(", ", list)
来源：http://nbz.hywenlv.cn

================================================================================
来源：http://iyv.zhaomingkeji.xyz

E. 字符串处理
来源：http://dqj.hnxiangtu.top

================================================================================
来源：http://qie.jinqigfzy.top

[E01] 拼接字符串
来源：http://zag.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ygr.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://usa.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnl.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://msv.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ghb.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jpr.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cfp.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jbz.vehdjk.com

[E02] 重复字符串
来源：http://dlo.daxiang520.top

Py:   "ab" * 3
来源：http://bmy.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://qdv.c1oappe.top

JS:   "ab".repeat(3)
来源：http://qdx.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://rvm.pycfn.com

Java: "ab".repeat(3)
来源：http://ner.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://srz.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://bbo.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yxf.yj202588.top

[E03] 截取子串
来源：http://pwc.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fpd.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fon.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fdv.uphjek.com

TS:   s.slice(1, 4)
来源：http://rii.guowangkeji.top

Java: s.substring(1, 4)
来源：http://vec.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jxd.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://msw.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://unq.jiagoushi.top

[E04] 查找子串位置
来源：http://yrr.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://voi.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://ldg.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kdr.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://qac.cashguo.top

Java: s.indexOf("x")
来源：http://vuo.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://nme.sxryk.cn

Ruby: s.index("x")
来源：http://dbt.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://pis.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bxf.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rot.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zgi.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnr.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dhr.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqw.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hun.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xkz.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wtv.yuxming.cn

[E06] 替换子串
来源：http://ynk.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fll.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://hyz.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isq.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://gmn.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kix.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cyb.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ysm.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://oxk.yvedp.cn

[E07] 按分隔符拆分
来源：http://civ.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnp.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gii.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wwg.cheryme.top

TS:   s.split(",")
来源：http://rbf.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://rfv.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zvp.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://leu.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kzp.yvedp.cn

[E08] 数组按分隔符合并
来源：http://uuh.chenjidiqi.icu

Py:   ",".join(items)
来源：http://orp.aibaodan.cn

PHP:  implode(",", $items);
来源：http://sgs.c1oappe.top

JS:   items.join(",")
来源：http://wnx.tian-w.cn

TS:   items.join(",")
来源：http://eic.ivvv.top

Java: String.join(",", items)
来源：http://jjt.yuxming.cn


<!-- 参考信息 -->