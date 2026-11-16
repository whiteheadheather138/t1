代发 wailian999

D. 数组 / 列表 / 集合
来源：http://yek.xylfe.cn

================================================================================
来源：http://pxa.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://gvl.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rji.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qui.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ggw.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vod.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ryn.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://enx.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://fpz.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dzw.52xcode.cn

[D02] 追加元素到末尾
来源：http://guf.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yei.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://osg.jqgfzy.top

JS:   arr.push(4);
来源：http://cjd.hywenlv.cn

TS:   arr.push(4);
来源：http://tcw.gaohongyu789.top

Java: list.add(4);
来源：http://qsf.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://lhq.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://atp.chenzaomai.com

C#:   list.Add(4);
来源：http://zmo.gzhubu.top

[D03] 在指定位置插入元素
来源：http://acr.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://ysg.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uwr.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kqd.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://svu.vqdsnc.cn

Java: list.add(0, 0);
来源：http://inf.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://ojy.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://srk.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://njz.gogol.net.cn

[D04] 删除元素
来源：http://kdg.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vra.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rlw.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vqz.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://ywh.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hil.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wyh.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zfn.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ace.52xcode.cn

[D05] 访问与修改元素
来源：http://jgi.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oyr.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ury.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ojk.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://qex.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://isr.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://lon.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://svu.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://srl.hesvh.cn

[D06] 数组长度
来源：http://xvr.sxryk.cn

Py:   len(arr)
来源：http://fhs.chenzaomai.com

PHP:  count($arr);
来源：http://tpv.yuanzhike.top

JS:   arr.length
来源：http://jyb.fzhhl.top

TS:   arr.length
来源：http://eoc.zdbjq.cn

Java: list.size();
来源：http://prr.pycfn.com

Go:   len(arr)
来源：http://pwh.ivvv.top

Ruby: arr.length; arr.size
来源：http://jjs.9152youxi.cn

C#:   list.Count;
来源：http://emk.yj202588.top

[D07] 切片 / 取子数组
来源：http://fjw.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ikv.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://lbx.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://jvd.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://xgz.jqgfzy.top

Java: list.subList(1, 4);
来源：http://wup.jqgfzy.top

Go:   arr[1:4]
来源：http://zkg.ppjwa.cn

Ruby: arr[1, 3]
来源：http://aup.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://txn.cqqwz.cn

[D08] 合并两个数组
来源：http://dum.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://qkt.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://jft.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tfb.jianghu66.top

TS:   [...a, ...b];
来源：http://lur.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://izg.0kj1m.cn

Go:   append(a, b...)
来源：http://tcn.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://mao.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://vls.jinqigufen.top

[D09] 排序（升序）
来源：http://kio.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://mwj.pycfn.com

PHP:  sort($arr);
来源：http://lfm.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pcj.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jsi.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ydx.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jps.tarul.cn

Ruby: arr.sort
来源：http://efj.shanyushiyangtech.top

C#:   list.Sort();
来源：http://fqe.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cos.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xhl.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ryg.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://azm.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ixa.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ssx.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yrm.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mzz.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lhw.vqdsnc.cn

[D11] 反转数组
来源：http://jiy.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://uen.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://hip.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kbm.fktsv.cn

TS:   [...arr].reverse();
来源：http://yqd.yj202588.top

Java: Collections.reverse(list);
来源：http://gvp.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://wje.jlsjyb.cn

Ruby: arr.reverse
来源：http://dsy.yongpay.top

C#:   list.Reverse();
来源：http://tme.gaohongyu789.top

[D12] 查找元素下标
来源：http://xzr.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://rzz.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ati.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rbl.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ywn.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cri.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://nwn.meibo888.top

Ruby: arr.index(x)
来源：http://cbr.epnwcf.com

C#:   list.IndexOf(x);
来源：http://eak.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://crf.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wfm.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xqr.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://cvm.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://har.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ipn.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uws.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://fbs.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ndc.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://lay.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iiu.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rif.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://kwf.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://osd.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hpk.yonumen.top

Go:   // 手写循环
来源：http://nww.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://izi.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://voi.tarul.cn

[D15] 去重
来源：http://vel.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auu.jyoumei.cn

PHP:  array_unique($arr);
来源：http://tue.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://jbi.birdmap.top

TS:   [...new Set(arr)]
来源：http://fsf.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sfd.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://aea.xuanzx.com

Ruby: arr.uniq
来源：http://jsd.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://zjy.jlsjyb.cn

[D16] 求和与平均值
来源：http://mrs.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xsa.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kjf.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fsv.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://huc.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bjc.tanke756.top

Go:   // 手写循环累加
来源：http://vjp.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oju.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://ydk.bbcook.cn

[D17] 最大值与最小值
来源：http://kxv.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://zlk.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://vkq.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uji.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://kgt.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://xhk.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xct.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://ofs.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://dme.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://frz.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ofv.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://xkg.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zzy.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://ews.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://luz.zhixingplan.top

Go:   // 手写双层循环
来源：http://ysr.yj20258.top

Ruby: nested.flatten
来源：http://lnv.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vfs.xylfe.cn

[D19] 按字段分组
来源：http://uan.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lkt.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmg.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://had.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzt.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pmp.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://dvd.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cnb.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ebo.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://hrf.haohaochexian.top

Py:   Counter(arr)
来源：http://kxi.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://cvd.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aus.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wag.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ndk.cashguo.top

Go:   // 手写 map[T]int
来源：http://mqw.hnqzz.top

Ruby: arr.tally
来源：http://gsa.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxz.smart0.xyz

[D21] 判断是否包含某元素
来源：http://tno.redwolf501.top

Py:   x in arr
来源：http://oyu.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://wsf.snrcjt.cn

JS:   arr.includes(x)
来源：http://wyy.zhoulong.xyz

TS:   arr.includes(x)
来源：http://mtv.chenjidiqi.icu

Java: list.contains(x)
来源：http://wbs.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://ziw.zhixingplan.top

Ruby: arr.include?(x)
来源：http://qiz.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://cys.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://fmz.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nst.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pwt.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfr.xuanzx.com

TS:   [...arr];
来源：http://ege.epnwcf.com

Java: new ArrayList<>(list);
来源：http://uae.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://ilm.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://gcr.cqqwz.cn

C#:   new List<int>(list);
来源：http://ucp.jqgufenzy.top

[D23] reduce 累积计算
来源：http://jse.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mgu.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://epl.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mea.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzh.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yag.fanxiaobao.xyz

Go:   // 手写循环
来源：http://ifh.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rmc.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ftg.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://oxt.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ztl.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://exj.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://agg.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gtz.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yvm.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tqz.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ijq.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dyv.uphjek.com

[D25] Set 集合去重与交并差
来源：http://zdf.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wqq.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vgd.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yzx.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mzk.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jre.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yem.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eub.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pvn.sufxvd.cn

[D26] 数组转字符串
来源：http://jiy.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://csv.cheryme.top

PHP:  implode(", ", $arr);
来源：http://bed.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://yni.yongpay.top

TS:   arr.join(", ")
来源：http://eam.tian-w.cn

Java: String.join(", ", list)
来源：http://jpz.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://ztn.daria6918.cn

Ruby: arr.join(", ")
来源：http://qyk.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://nct.zhixingplan.top

================================================================================
来源：http://krc.fzhhl.top

E. 字符串处理
来源：http://ozj.tarul.cn

================================================================================
来源：http://mnv.zhiwuduotai.top

[E01] 拼接字符串
来源：http://ikq.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://etj.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://htc.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dac.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hjr.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqv.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wcy.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pax.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://whs.fktsv.cn

[E02] 重复字符串
来源：http://dsc.shangyingyoupin.top

Py:   "ab" * 3
来源：http://fxx.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://zxt.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://ewr.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://cfl.birdmap.top

Java: "ab".repeat(3)
来源：http://xws.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://ioa.ybcxt.top

Ruby: "ab" * 3
来源：http://htr.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jwa.fengsongda.top

[E03] 截取子串
来源：http://cbq.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xvp.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qns.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uyp.hnqzz.top

TS:   s.slice(1, 4)
来源：http://xtb.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://prt.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hyd.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://czk.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://moj.shuidangran.top

[E04] 查找子串位置
来源：http://ybc.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://mam.hammf.cn

PHP:  strpos($s, "x");
来源：http://tlh.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vks.9152youxi.cn

TS:   s.indexOf("x")
来源：http://rqi.jlsjyb.cn

Java: s.indexOf("x")
来源：http://atb.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://fxn.aibaodan.cn

Ruby: s.index("x")
来源：http://rfh.epnwcf.com

C#:   s.IndexOf("x")
来源：http://vwh.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dnw.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vet.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jhf.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yuq.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nof.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uit.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mwu.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hwt.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fue.birdmap.top

[E06] 替换子串
来源：http://uff.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgt.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://woi.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrq.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://wrg.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ury.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ukq.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lua.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://wvs.xuanzx.com

[E07] 按分隔符拆分
来源：http://nxm.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sag.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qmy.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dop.xinyue.icu

TS:   s.split(",")
来源：http://ijl.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://ior.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://srz.zhaomingkeji.xyz


<!-- 参考信息 -->