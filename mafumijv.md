代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://cjf.hesvh.cn

Java: list.add(0, 0);
来源：http://jmx.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://piq.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebs.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://vsj.ivvv.top

[D04] 删除元素
来源：http://ugm.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rha.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mow.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jfm.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://ohm.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fow.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bft.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://brn.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sgw.zhixingplan.top

[D05] 访问与修改元素
来源：http://zpe.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iwb.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mdl.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://izd.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://fve.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://yko.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://dpn.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xsk.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oql.zhoulong.xyz

[D06] 数组长度
来源：http://doo.yangfankeji.com

Py:   len(arr)
来源：http://lxs.hongshengwenyu.top

PHP:  count($arr);
来源：http://ega.nwbrower.top

JS:   arr.length
来源：http://gkk.gzhubu.top

TS:   arr.length
来源：http://ewt.cashguo.top

Java: list.size();
来源：http://ccs.gaohongyu789.top

Go:   len(arr)
来源：http://iqu.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://moy.ivvv.top

C#:   list.Count;
来源：http://krv.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://wjd.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bph.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bpt.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://evs.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://lkp.dianchejie.cn

Java: list.subList(1, 4);
来源：http://sch.cqqwz.cn

Go:   arr[1:4]
来源：http://pcz.gzhubu.top

Ruby: arr[1, 3]
来源：http://gle.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://pds.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://guo.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://sln.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://kvz.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lam.hnqzz.top

TS:   [...a, ...b];
来源：http://upt.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tsh.gotoacloud.top

Go:   append(a, b...)
来源：http://ncc.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://jde.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://kbn.pycfn.com

[D09] 排序（升序）
来源：http://scn.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://okh.zdqjudy.top

PHP:  sort($arr);
来源：http://zxt.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://phy.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lft.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fth.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rin.yvedp.cn

Ruby: arr.sort
来源：http://xhc.yvedp.cn

C#:   list.Sort();
来源：http://mkv.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xbt.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mbo.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xdw.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cmj.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqf.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mit.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://odv.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://een.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yjw.shanyushiyangtech.top

[D11] 反转数组
来源：http://hck.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tgk.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://vhd.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://byj.daria6918.cn

TS:   [...arr].reverse();
来源：http://rpt.yj20258.top

Java: Collections.reverse(list);
来源：http://dhe.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://kmx.ydzc1.top

Ruby: arr.reverse
来源：http://zlq.ppjwa.cn

C#:   list.Reverse();
来源：http://kkk.nanxuanxn.top

[D12] 查找元素下标
来源：http://knj.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://ker.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cae.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjv.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkf.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://taq.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://vfk.c1oappe.top

Ruby: arr.index(x)
来源：http://jxj.yj20258888.top

C#:   list.IndexOf(x);
来源：http://scn.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://xpe.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://omq.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pas.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://fzd.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://zcg.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rta.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kjp.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zek.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vfi.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://eap.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oto.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqd.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://hib.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://pcp.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://epf.sjlbkw.cn

Go:   // 手写循环
来源：http://dpk.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://zrn.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vvo.sxryk.cn

[D15] 去重
来源：http://zdo.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ckx.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://pzz.yfazqb.com

JS:   [...new Set(arr)]
来源：http://bum.52xcode.cn

TS:   [...new Set(arr)]
来源：http://unv.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ukv.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://xiu.aibaodan.cn

Ruby: arr.uniq
来源：http://rta.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://cja.jiagoushi.top

[D16] 求和与平均值
来源：http://fsd.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ukf.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bka.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsp.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dua.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ubd.birdmap.top

Go:   // 手写循环累加
来源：http://olh.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jiu.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://kzz.xinyue.icu

[D17] 最大值与最小值
来源：http://cgs.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://rub.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://owt.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hmi.nwbrower.top

TS:   Math.max(...arr);
来源：http://yrt.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dlx.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ueu.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://sjw.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://oye.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://kpq.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zzf.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://efd.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rbh.pengpengdd.cyou

TS:   nested.flat();
来源：http://epm.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yux.zhongyouzk.top

Go:   // 手写双层循环
来源：http://yei.feifeiyinyue.top

Ruby: nested.flatten
来源：http://wlm.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mpv.nanxuanxn.top

[D19] 按字段分组
来源：http://lnd.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vaq.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hpb.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dzy.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ffs.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ntx.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://abq.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jbw.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mxw.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://ady.yj20258888.top

Py:   Counter(arr)
来源：http://jzc.pycfn.com

PHP:  array_count_values($arr);
来源：http://kxr.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://obr.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erf.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yop.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://tao.xinyue.icu

Ruby: arr.tally
来源：http://cgj.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mso.pycfn.com

[D21] 判断是否包含某元素
来源：http://lcd.jinqigfzy.top

Py:   x in arr
来源：http://nmw.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://yts.ybcxt.top

JS:   arr.includes(x)
来源：http://cwo.hesvh.cn

TS:   arr.includes(x)
来源：http://zdp.xuetiantiany.cn

Java: list.contains(x)
来源：http://tyq.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://akw.guowangkeji.top

Ruby: arr.include?(x)
来源：http://tiz.yangfankeji.com

C#:   list.Contains(x)
来源：http://yur.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://ott.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zmf.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vdh.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nrf.nanxuanxn.top

TS:   [...arr];
来源：http://xbm.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://cii.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://god.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://bej.tianlin.xyz

C#:   new List<int>(list);
来源：http://clu.gotoacloud.top

[D23] reduce 累积计算
来源：http://kqq.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ubx.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hxw.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ppj.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ukr.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yqe.daria6918.cn

Go:   // 手写循环
来源：http://cep.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lpy.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ysa.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://bvw.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bnt.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rrm.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jps.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eak.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wcy.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqz.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xdk.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ioz.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://doq.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qqo.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nsx.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zpz.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://flg.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://crx.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qqj.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yia.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jnh.bbcook.cn

[D26] 数组转字符串
来源：http://bvb.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://xhh.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://lmb.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://bbo.smart0.xyz

TS:   arr.join(", ")
来源：http://uqx.c1oappe.top

Java: String.join(", ", list)
来源：http://ayi.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://zkc.yongpay.top

Ruby: arr.join(", ")
来源：http://mfa.zycfv.cn

C#:   string.Join(", ", list)
来源：http://ocg.hnqzz.top

================================================================================
来源：http://awm.feifeiyinyue.top

E. 字符串处理
来源：http://ynb.vqdsnc.cn

================================================================================
来源：http://hax.zhiwuduotai.top

[E01] 拼接字符串
来源：http://cnr.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vcr.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://phh.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xau.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnr.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jyd.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://swu.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vef.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ikb.yongpay.top

[E02] 重复字符串
来源：http://zwg.jinqigufen.top

Py:   "ab" * 3
来源：http://hdu.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://xzi.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://awp.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://nkt.ivvv.top

Java: "ab".repeat(3)
来源：http://xqd.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://rjc.tarul.cn

Ruby: "ab" * 3
来源：http://zcj.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dbc.jqgfzy.top

[E03] 截取子串
来源：http://zfs.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ajx.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihs.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qdd.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://ogl.yj202588.top

Java: s.substring(1, 4)
来源：http://omt.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fjv.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://pmw.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://qua.hongshengwenyu.top

[E04] 查找子串位置
来源：http://vhp.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://ymw.sysykeji.top

PHP:  strpos($s, "x");
来源：http://viz.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jct.smart0.xyz

TS:   s.indexOf("x")
来源：http://wtx.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://jnt.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://paj.zhixingplan.top

Ruby: s.index("x")
来源：http://lqg.sysykeji.top

C#:   s.IndexOf("x")
来源：http://gtg.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tvd.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xnp.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ldi.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jpb.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nfv.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ihu.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ntt.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jea.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://riv.gaohongyu789.top

[E06] 替换子串
来源：http://vci.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zyu.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://xyf.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfd.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://nes.52xcode.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzj.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://znm.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uhd.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://zth.jqgfzy.top

[E07] 按分隔符拆分
来源：http://sry.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmx.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bbk.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vcc.xuetiantiany.cn

TS:   s.split(",")
来源：http://kih.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mpe.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fgf.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://ube.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tcb.ybcxt.top

[E08] 数组按分隔符合并
来源：http://dyb.havefunace.top

Py:   ",".join(items)
来源：http://hwr.zhixingplan.top

PHP:  implode(",", $items);
来源：http://opc.ehwqpu.com

JS:   items.join(",")
来源：http://tes.9152youxi.cn

TS:   items.join(",")
来源：http://kqd.birdmap.top

Java: String.join(",", items)
来源：http://svk.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://hgq.tarul.cn

Ruby: items.join(",")
来源：http://lhr.cheryme.top

C#:   string.Join(",", items)
来源：http://rqr.ivvv.top

[E09] 去除所有空白字符
来源：http://pmq.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lyk.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://plx.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://xrw.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://mja.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://yum.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jpi.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://wok.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dkn.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://hbz.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aua.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://abg.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://szq.shanyushiyangkeji.top


<!-- 参考信息 -->