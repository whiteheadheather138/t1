代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://kxj.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://fns.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ebu.jinqigufen.top

================================================================================
来源：http://bnu.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://fkl.bjfxy.top

================================================================================
来源：http://wfa.hcnkem.com

[D01] 创建数组 / 列表
来源：http://gpn.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qdj.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hee.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vjn.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://diy.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gys.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://rld.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://vfm.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kzj.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://wqk.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mpt.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://muk.xinyue.icu

JS:   arr.push(4);
来源：http://ykj.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://kkf.gotoacloud.top

Java: list.add(4);
来源：http://rps.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://phj.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://zxw.nanxuanxn.top

C#:   list.Add(4);
来源：http://nzx.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://cfb.ivvv.top

Py:   arr.insert(0, 0)
来源：http://alt.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zct.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sfx.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://vag.guannengcc.top

Java: list.add(0, 0);
来源：http://bms.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://rlw.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zuv.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://hmj.wangshuangyany.cn

[D04] 删除元素
来源：http://ntu.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqn.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ajj.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tet.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://vij.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eyl.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uco.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usq.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eag.shuidangran.top

[D05] 访问与修改元素
来源：http://tcl.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmf.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jen.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bwv.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://tcn.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://fww.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://amf.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://moh.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://swl.9152youxi.cn

[D06] 数组长度
来源：http://ruy.zdbjq.cn

Py:   len(arr)
来源：http://ads.c1oappe.top

PHP:  count($arr);
来源：http://ora.yj20258888.top

JS:   arr.length
来源：http://zhy.jiagoushi.top

TS:   arr.length
来源：http://hbi.zhengqikj.top

Java: list.size();
来源：http://dks.xuetiantiany.cn

Go:   len(arr)
来源：http://lsy.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://zbt.yongpay.top

C#:   list.Count;
来源：http://grd.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://imk.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://apq.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wwf.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://rew.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://rdg.ehwqpu.com

Java: list.subList(1, 4);
来源：http://llq.tarul.cn

Go:   arr[1:4]
来源：http://jmm.ivvv.top

Ruby: arr[1, 3]
来源：http://ioa.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://ryf.meibo888.top

[D08] 合并两个数组
来源：http://rew.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://lps.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://qoy.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://quz.haohaochexian.top

TS:   [...a, ...b];
来源：http://nrt.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zml.birdmap.top

Go:   append(a, b...)
来源：http://fmk.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://gua.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://yhm.pengpengdd.cyou

[D09] 排序（升序）
来源：http://mwd.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://qbs.cucudq.cn

PHP:  sort($arr);
来源：http://kun.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wxl.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wjm.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vlk.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://snj.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://ewy.tianlin.xyz

C#:   list.Sort();
来源：http://hec.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aiq.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vrt.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oke.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ubh.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dtq.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aho.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rlj.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uas.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xwx.andypj.xyz

[D11] 反转数组
来源：http://hzy.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://sfa.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://nsn.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fnl.haohaochexian.top

TS:   [...arr].reverse();
来源：http://ddq.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://yvq.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://laq.52xcode.cn

Ruby: arr.reverse
来源：http://gnu.sjlbkw.cn

C#:   list.Reverse();
来源：http://xiq.andypj.xyz

[D12] 查找元素下标
来源：http://vgd.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://pbf.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sws.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrw.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nya.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rjs.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://igp.jlsjyb.cn

Ruby: arr.index(x)
来源：http://gkb.tarul.cn

C#:   list.IndexOf(x);
来源：http://osb.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://hbp.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rcz.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://deh.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://dlv.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://yzs.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nlv.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xgq.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://kbp.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ngv.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://epe.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gou.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lwt.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://emu.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://xdp.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hat.sweek.top

Go:   // 手写循环
来源：http://ova.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qfz.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tok.gogol.net.cn

[D15] 去重
来源：http://dec.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rzm.iojbl.cn

PHP:  array_unique($arr);
来源：http://xta.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://fhl.pycfn.com

TS:   [...new Set(arr)]
来源：http://jkd.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sqr.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dte.shuidangran.top

Ruby: arr.uniq
来源：http://qrn.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://yqc.hysaishi.cn

[D16] 求和与平均值
来源：http://eyh.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://myq.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://btn.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iki.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://coc.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rax.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://ock.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvi.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://hii.zdqjudy.top

[D17] 最大值与最小值
来源：http://wko.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://nrx.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://hgd.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://adr.xziqi.cn

TS:   Math.max(...arr);
来源：http://gcd.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pkd.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xde.pycfn.com

Ruby: arr.max;  arr.min
来源：http://lwq.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://kyw.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://hrr.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qir.yj20258.top

PHP:  array_merge(...$nested);
来源：http://sdf.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qxw.fktsv.cn

TS:   nested.flat();
来源：http://bol.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mrw.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://vqy.c1oappe.top

Ruby: nested.flatten
来源：http://gpa.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pka.bjfxy.top

[D19] 按字段分组
来源：http://qtp.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edo.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://awn.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://avs.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mvu.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aez.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://jgo.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://psd.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zix.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://rik.tarul.cn

Py:   Counter(arr)
来源：http://opv.andypj.xyz

PHP:  array_count_values($arr);
来源：http://cae.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qac.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qcw.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jdu.c1oappe.top

Go:   // 手写 map[T]int
来源：http://wpr.bbcook.cn

Ruby: arr.tally
来源：http://hfu.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qja.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://cvo.wangshuangyany.cn

Py:   x in arr
来源：http://cfk.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://yhx.zycfv.cn

JS:   arr.includes(x)
来源：http://qtk.xinyue.icu

TS:   arr.includes(x)
来源：http://toy.hysaishi.cn

Java: list.contains(x)
来源：http://nms.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://gjz.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://aja.fengsongda.top

C#:   list.Contains(x)
来源：http://ulb.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://haj.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bqb.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://itc.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kta.sysykeji.top

TS:   [...arr];
来源：http://fmj.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://qhx.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iuy.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://znq.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://fdb.epnwcf.com

[D23] reduce 累积计算
来源：http://yxb.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eyx.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://abp.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zie.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://juc.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://snd.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://njd.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hhz.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bsv.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://dxw.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohl.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://usj.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://amz.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aww.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yga.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xgf.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vcc.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uuc.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://xlm.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejt.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jih.fehbvm.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nlh.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xjd.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gln.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iyk.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dab.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jil.wangdashe.top

[D26] 数组转字符串
来源：http://zgi.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://qxo.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://vlv.fengsongda.top

JS:   arr.join(", ")
来源：http://rqa.jiagoushi.top

TS:   arr.join(", ")
来源：http://rmf.havefunace.top

Java: String.join(", ", list)
来源：http://who.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://wda.daxiang520.top

Ruby: arr.join(", ")
来源：http://lly.xinyue.icu

C#:   string.Join(", ", list)
来源：http://ljz.yj20258.top

================================================================================
来源：http://god.zhengqikj.top

E. 字符串处理
来源：http://crf.yj20258888.top

================================================================================
来源：http://zhj.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://xwz.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pri.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://scp.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwu.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kny.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jrg.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wbc.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwo.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tst.tianlin.xyz

[E02] 重复字符串
来源：http://nwh.snrcjt.cn

Py:   "ab" * 3
来源：http://ces.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://zvd.hammf.cn

JS:   "ab".repeat(3)
来源：http://xch.uphjek.com

TS:   "ab".repeat(3)
来源：http://amr.cheryme.top

Java: "ab".repeat(3)
来源：http://xav.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://oyt.316326.xyz

Ruby: "ab" * 3
来源：http://nvy.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dno.gotoacloud.top

[E03] 截取子串
来源：http://yyx.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dbq.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lmb.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://khc.hnqzz.top

TS:   s.slice(1, 4)
来源：http://flg.sxryk.cn

Java: s.substring(1, 4)
来源：http://ikm.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dtv.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gzr.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://fir.sweek.top

[E04] 查找子串位置
来源：http://yps.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://bht.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://uef.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dhx.bbcook.cn

TS:   s.indexOf("x")
来源：http://hdm.gotoacloud.top

Java: s.indexOf("x")
来源：http://vqh.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://lhr.iojbl.cn

Ruby: s.index("x")
来源：http://vhh.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://oqx.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hzr.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ikv.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dbx.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lbl.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ubl.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mnf.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pdk.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ywr.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iqe.mhx1999.top

[E06] 替换子串
来源：http://vtc.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zee.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://gwk.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rph.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://qbz.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://anh.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zdw.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vpf.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://tzh.zdqjudy.top

[E07] 按分隔符拆分
来源：http://dru.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vky.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bda.chenjidiqi.icu


<!-- 参考信息 -->