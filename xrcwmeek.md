代发 wailian999

Ruby: a, b = pair
来源：http://gwn.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://wap.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://kja.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mcn.nanxuanxn.top

PHP:  // 无重载
来源：http://bes.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cbr.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://kbh.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://nri.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://hgp.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://qko.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wwx.fktsv.cn

================================================================================
来源：http://pdt.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://tfe.gotoacloud.top

================================================================================
来源：http://zxj.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://gph.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wrl.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xvt.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://urm.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vne.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://val.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://syw.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://hkp.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jgv.yonumen.top

[D02] 追加元素到末尾
来源：http://qjl.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kej.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gus.gotoacloud.top

JS:   arr.push(4);
来源：http://afa.jqgfzy.top

TS:   arr.push(4);
来源：http://oru.jinyuanbaomall.cn

Java: list.add(4);
来源：http://htv.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://zdn.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://art.zhixingplan.top

C#:   list.Add(4);
来源：http://ktg.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://lbj.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://pbn.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cdi.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tec.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://ngw.jinqigfzy.top

Java: list.add(0, 0);
来源：http://ehy.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://knn.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmi.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://tow.c1oappe.top

[D04] 删除元素
来源：http://znp.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://upk.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fdx.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yqg.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://buw.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tkr.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xxa.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ucr.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://esq.bjfxy.top

[D05] 访问与修改元素
来源：http://vmq.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nug.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bcc.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gdt.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://ybr.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://aqj.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://ofe.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lbd.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hgf.9152youxi.cn

[D06] 数组长度
来源：http://zwl.gzhubu.top

Py:   len(arr)
来源：http://dox.guannengcc.top

PHP:  count($arr);
来源：http://tvi.jlsjyb.cn

JS:   arr.length
来源：http://pux.zhijiandao.cn

TS:   arr.length
来源：http://tyf.gzhubu.top

Java: list.size();
来源：http://eot.ehwqpu.com

Go:   len(arr)
来源：http://fkc.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://kei.fktsv.cn

C#:   list.Count;
来源：http://ndb.zycfv.cn

[D07] 切片 / 取子数组
来源：http://zgp.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xib.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zmy.havefunace.top

JS:   arr.slice(1, 4);
来源：http://ksz.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://rqv.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://lhk.epnwcf.com

Go:   arr[1:4]
来源：http://org.ctjpmb.com

Ruby: arr[1, 3]
来源：http://aip.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://zll.jinqigfzy.top

[D08] 合并两个数组
来源：http://anr.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://hnz.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://kcg.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rgg.dianchejie.cn

TS:   [...a, ...b];
来源：http://kvc.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uxc.yfazqb.com

Go:   append(a, b...)
来源：http://oha.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://ksv.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://wke.shangyingyoupin.top

[D09] 排序（升序）
来源：http://ete.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://hql.zhiwuduotai.top

PHP:  sort($arr);
来源：http://fby.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ykf.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://vcf.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mzr.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfi.iojbl.cn

Ruby: arr.sort
来源：http://bgj.gaohongyu789.top

C#:   list.Sort();
来源：http://dhv.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kjh.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eaq.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://igp.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vhe.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://chz.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvo.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dcu.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xjl.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://til.jianghu66.top

[D11] 反转数组
来源：http://cle.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://zvo.yj20258.top

PHP:  array_reverse($arr);
来源：http://pya.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jmu.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://wir.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://wfi.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://inc.pycfn.com

Ruby: arr.reverse
来源：http://xcx.svipenyu.cn

C#:   list.Reverse();
来源：http://wdj.snrcjt.cn

[D12] 查找元素下标
来源：http://aiy.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://mnl.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tei.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tcf.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ijo.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifq.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://jyh.zhengqikj.top

Ruby: arr.index(x)
来源：http://vvm.yj20258.top

C#:   list.IndexOf(x);
来源：http://hpp.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://hsz.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lvu.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lre.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://mqi.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://iem.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bim.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jip.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://wmm.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kcz.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://hnl.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aen.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cgg.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://epz.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://dcj.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nad.yueranfly.top

Go:   // 手写循环
来源：http://bmk.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://hiq.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mwn.52xcode.cn

[D15] 去重
来源：http://mdz.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://thn.vehdjk.com

PHP:  array_unique($arr);
来源：http://blm.hammf.cn

JS:   [...new Set(arr)]
来源：http://gre.yonumen.top

TS:   [...new Set(arr)]
来源：http://coe.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mng.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vvq.daria6918.cn

Ruby: arr.uniq
来源：http://dey.havefunace.top

C#:   list.Distinct().ToList()
来源：http://dvn.zhengqikj.top

[D16] 求和与平均值
来源：http://axw.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fdh.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xmr.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://izr.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfd.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://alz.fehbvm.com

Go:   // 手写循环累加
来源：http://jsb.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://smu.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://nam.cucudq.cn

[D17] 最大值与最小值
来源：http://uzh.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://ucw.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://eim.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aqx.dianchejie.cn

TS:   Math.max(...arr);
来源：http://rgu.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ejo.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jji.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://ehz.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://ocr.havefunace.top

[D18] 扁平化嵌套数组
来源：http://hux.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ibu.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://ntl.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owh.aibaodan.cn

TS:   nested.flat();
来源：http://vdq.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gcy.chenlongwang.top

Go:   // 手写双层循环
来源：http://gcv.xuanzx.com

Ruby: nested.flatten
来源：http://npt.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zeb.jlsjyb.cn

[D19] 按字段分组
来源：http://dxe.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pgj.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://opz.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://abw.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jvl.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xer.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://xzp.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://saz.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nah.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://tkb.jqgufenzy.top

Py:   Counter(arr)
来源：http://fda.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://hel.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://due.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cnz.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mdx.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://vor.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://brj.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mzj.hcnkem.com

[D21] 判断是否包含某元素
来源：http://eei.gogol.net.cn

Py:   x in arr
来源：http://ihn.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://xqo.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://vld.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://zfn.bjfxy.top

Java: list.contains(x)
来源：http://mzt.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://ysi.sysykeji.top

Ruby: arr.include?(x)
来源：http://vxp.sufxvd.cn

C#:   list.Contains(x)
来源：http://ffi.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://fnw.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dhf.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gcg.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qpi.nwbrower.top

TS:   [...arr];
来源：http://sto.tian-w.cn

Java: new ArrayList<>(list);
来源：http://wtd.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ugi.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://psi.ydjk.org.cn

C#:   new List<int>(list);
来源：http://zrw.yj20258888.top

[D23] reduce 累积计算
来源：http://zxn.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ogi.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fsv.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yzu.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ejc.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uxc.snrcjt.cn

Go:   // 手写循环
来源：http://dll.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aaf.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctl.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://ozf.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ntn.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cfy.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gah.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aky.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ltb.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rvi.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dcn.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tko.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://eve.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://alx.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xty.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kwo.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nth.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fnw.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nfy.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qaj.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zxo.cdnleiting.top

[D26] 数组转字符串
来源：http://irh.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://jbv.0kj1m.cn

PHP:  implode(", ", $arr);
来源：http://cua.tanke756.top

JS:   arr.join(", ")
来源：http://gcq.cheryme.top

TS:   arr.join(", ")
来源：http://kyq.yfazqb.com

Java: String.join(", ", list)
来源：http://gau.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://ojs.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://vej.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://ccp.iojbl.cn

================================================================================
来源：http://bla.iojbl.cn

E. 字符串处理
来源：http://aww.sysykeji.top

================================================================================
来源：http://nss.jinqigufen.top

[E01] 拼接字符串
来源：http://zxg.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iul.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fud.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgs.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wam.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lwf.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pcp.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqs.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iwl.xziqi.cn

[E02] 重复字符串
来源：http://qry.aizwys.cn

Py:   "ab" * 3
来源：http://jgp.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://buf.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://bnw.yueranfly.top

TS:   "ab".repeat(3)
来源：http://qlp.yj20258.top

Java: "ab".repeat(3)
来源：http://mah.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://vbk.zdbjq.cn

Ruby: "ab" * 3
来源：http://wli.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fkz.zycfv.cn

[E03] 截取子串
来源：http://kvj.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://olq.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xzb.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eiy.daria6918.cn

TS:   s.slice(1, 4)
来源：http://ldn.chenzaomai.com

Java: s.substring(1, 4)
来源：http://inv.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://inx.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ykv.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://hne.chenzaomai.com

[E04] 查找子串位置
来源：http://ekp.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://myr.cucudq.cn

PHP:  strpos($s, "x");
来源：http://kle.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dza.dianchejie.cn

TS:   s.indexOf("x")
来源：http://vqf.ybcxt.top

Java: s.indexOf("x")
来源：http://zfq.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://xmt.ppjwa.cn

Ruby: s.index("x")
来源：http://ljo.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://uux.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dal.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jvr.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bbq.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imb.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pay.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cia.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://flf.fanxiaobao.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rnd.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nmv.haohaochexian.top

[E06] 替换子串
来源：http://nwr.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzs.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://fdm.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lqx.birdmap.top


<!-- 参考信息 -->