代发 wailian999

Ruby: a, b = pair
来源：http://fqj.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://uwf.wangdashe.top

[C16] 函数 / 方法重载
来源：http://her.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://plx.ctjpmb.com

PHP:  // 无重载
来源：http://hty.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hty.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://vzp.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vcg.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://vrl.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://rpf.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hfx.hnxiangtu.top

================================================================================
来源：http://wlf.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://ile.chenlongwang.top

================================================================================
来源：http://glc.c1oappe.top

[D01] 创建数组 / 列表
来源：http://dpv.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vhw.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ezp.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fpc.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rns.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gob.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://cby.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://dbm.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zvs.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://fsb.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://inw.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://otf.shangyingyoupin.top

JS:   arr.push(4);
来源：http://zjr.hesvh.cn

TS:   arr.push(4);
来源：http://dlf.ehwqpu.com

Java: list.add(4);
来源：http://ogr.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://wbk.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ual.chenzaomai.com

C#:   list.Add(4);
来源：http://fnt.yonumen.top

[D03] 在指定位置插入元素
来源：http://qtk.yonumen.top

Py:   arr.insert(0, 0)
来源：http://fha.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aof.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yji.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://mhe.ydjk.org.cn

Java: list.add(0, 0);
来源：http://teb.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://hyn.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ppn.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://glx.hywenlv.cn

[D04] 删除元素
来源：http://eff.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ava.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://avu.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vfw.tarul.cn

TS:   arr.splice(0, 1);
来源：http://bim.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jlh.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpx.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zsf.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pgl.jinqigufen.top

[D05] 访问与修改元素
来源：http://njd.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mdv.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kjs.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gkz.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://dsq.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://rad.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://mwa.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rrj.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hvw.cdnleiting.top

[D06] 数组长度
来源：http://hfc.wangshuangyany.cn

Py:   len(arr)
来源：http://cxo.hongshengwenyu.top

PHP:  count($arr);
来源：http://dtr.uphjek.com

JS:   arr.length
来源：http://eum.wangshuangyany.cn

TS:   arr.length
来源：http://kqy.hfpthk.cn

Java: list.size();
来源：http://clz.yangfankeji.com

Go:   len(arr)
来源：http://uhk.uphjek.com

Ruby: arr.length; arr.size
来源：http://lwx.yuxming.cn

C#:   list.Count;
来源：http://hyq.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ldo.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hak.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zin.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://eou.meibo888.top

TS:   arr.slice(1, 4);
来源：http://mtt.yongpay.top

Java: list.subList(1, 4);
来源：http://qbk.316326.xyz

Go:   arr[1:4]
来源：http://pvp.gzhubu.top

Ruby: arr[1, 3]
来源：http://lef.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://ten.sweek.top

[D08] 合并两个数组
来源：http://fvx.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://vgc.birdmap.top

PHP:  array_merge($a, $b);
来源：http://lsw.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://deu.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://yfg.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vic.sjlbkw.cn

Go:   append(a, b...)
来源：http://zwr.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://ymr.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://xqp.dashuyun.cn

[D09] 排序（升序）
来源：http://ueo.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://akk.feifeiyinyue.top

PHP:  sort($arr);
来源：http://ylq.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qrj.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://naw.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://afu.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://teb.yj20258888.top

Ruby: arr.sort
来源：http://zuy.yuanzhike.top

C#:   list.Sort();
来源：http://nqg.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://qvp.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ayv.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrn.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cum.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xwe.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://smw.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ear.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://igi.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nzl.yj20258888.top

[D11] 反转数组
来源：http://gge.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://tnn.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://qqa.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://atn.yonumen.top

TS:   [...arr].reverse();
来源：http://krz.c1oappe.top

Java: Collections.reverse(list);
来源：http://adb.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://zpb.yueranfly.top

Ruby: arr.reverse
来源：http://bpc.gzhubu.top

C#:   list.Reverse();
来源：http://vjr.shangyingyoupin.top

[D12] 查找元素下标
来源：http://tfr.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://jdo.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nae.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmc.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rta.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ygc.yj202588.top

Go:   slices.Index(arr, x)
来源：http://uyf.yj202588.top

Ruby: arr.index(x)
来源：http://ekr.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://pjc.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://zmi.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iai.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eef.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://eji.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://voz.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://adr.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zdg.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://qng.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xto.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://hgu.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vnh.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ivn.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://qqz.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://asn.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kqp.cdnleiting.top

Go:   // 手写循环
来源：http://kmd.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bvr.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uzl.nwbrower.top

[D15] 去重
来源：http://zzh.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xis.daria6918.cn

PHP:  array_unique($arr);
来源：http://jvn.hnqzz.top

JS:   [...new Set(arr)]
来源：http://fan.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://bxd.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dom.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://kdu.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://gqk.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://skc.haohaochexian.top

[D16] 求和与平均值
来源：http://vpf.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fkx.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://osd.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fqf.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsb.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nfe.xinyue.icu

Go:   // 手写循环累加
来源：http://cmu.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bvr.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://ros.hywenlv.cn

[D17] 最大值与最小值
来源：http://wgy.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://wvb.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://xea.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://frf.vehdjk.com

TS:   Math.max(...arr);
来源：http://ntn.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wau.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xte.tanke756.top

Ruby: arr.max;  arr.min
来源：http://jmy.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://fig.316326.xyz

[D18] 扁平化嵌套数组
来源：http://xnp.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdg.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://onq.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wku.jinqigfzy.top

TS:   nested.flat();
来源：http://dje.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wml.aizwys.cn

Go:   // 手写双层循环
来源：http://glm.meibo888.top

Ruby: nested.flatten
来源：http://zuw.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sdq.quarkkingdee.top

[D19] 按字段分组
来源：http://tza.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mgo.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ojm.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lno.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wkb.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qck.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://hkk.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lbx.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cnr.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://jnw.guowangkeji.top

Py:   Counter(arr)
来源：http://mtx.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://dur.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dve.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aot.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mjx.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://tzm.nwbrower.top

Ruby: arr.tally
来源：http://kug.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xiw.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://beq.daria6918.cn

Py:   x in arr
来源：http://pwo.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://llf.cheryme.top

JS:   arr.includes(x)
来源：http://xqj.zhoulong.xyz

TS:   arr.includes(x)
来源：http://mtx.hongshengwenyu.top

Java: list.contains(x)
来源：http://koa.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://wxw.cucudq.cn

Ruby: arr.include?(x)
来源：http://mlz.ydjk.org.cn

C#:   list.Contains(x)
来源：http://vur.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://xnc.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fso.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hrf.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eny.shanyushiyangkeji.top

TS:   [...arr];
来源：http://gso.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://rzl.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://aus.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://hrj.jqgfzy.top

C#:   new List<int>(list);
来源：http://yaj.zdbjq.cn

[D23] reduce 累积计算
来源：http://pgk.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kxq.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://srn.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpm.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vle.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxu.dianchejie.cn

Go:   // 手写循环
来源：http://fme.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://woy.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aur.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://cee.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eru.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tjr.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://guw.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://moz.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mhw.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jce.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jth.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dbd.yongpay.top

[D25] Set 集合去重与交并差
来源：http://qwx.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gyp.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wxk.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kro.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fdf.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dao.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://asb.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vrq.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ioh.wangshuangyany.cn

[D26] 数组转字符串
来源：http://edm.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://hbj.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://iod.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://mkw.yueranfly.top

TS:   arr.join(", ")
来源：http://wpq.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://ghd.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://rkf.andypj.xyz

Ruby: arr.join(", ")
来源：http://hve.meibo888.top

C#:   string.Join(", ", list)
来源：http://ocs.9152youxi.cn

================================================================================
来源：http://flj.xuetiantiany.cn

E. 字符串处理
来源：http://vlp.hongshengwenyu.top

================================================================================
来源：http://xsh.zycfv.cn

[E01] 拼接字符串
来源：http://ord.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gqi.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ynw.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kxk.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vjw.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gpw.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bpr.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fgt.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxu.316326.xyz

[E02] 重复字符串
来源：http://vxn.nanxinkj.top

Py:   "ab" * 3
来源：http://bvq.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://bye.cheryme.top

JS:   "ab".repeat(3)
来源：http://ytj.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://chk.bbcook.cn

Java: "ab".repeat(3)
来源：http://dix.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://lli.sufxvd.cn

Ruby: "ab" * 3
来源：http://feh.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pyc.xylfe.cn

[E03] 截取子串
来源：http://esp.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kwv.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aha.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://biw.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://gwn.fehbvm.com

Java: s.substring(1, 4)
来源：http://jou.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jlp.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fca.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://uuc.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://ocb.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://eza.hcnkem.com

PHP:  strpos($s, "x");
来源：http://gkp.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mit.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://cfe.wangdashe.top

Java: s.indexOf("x")
来源：http://xpv.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://ily.hammf.cn

Ruby: s.index("x")
来源：http://upk.gzhubu.top

C#:   s.IndexOf("x")
来源：http://ejc.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yvx.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gmh.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mex.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rci.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://urv.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iyz.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gok.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gbd.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gjv.wangdashe.top

[E06] 替换子串
来源：http://otn.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gsk.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://wws.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfc.hysaishi.cn


<!-- 参考信息 -->