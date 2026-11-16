代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czl.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rpr.jqgfzy.top

Java: // 无解构
来源：http://umz.ywan-chungtsiang.top

Go:   // 无解构
来源：http://kmf.havefunace.top

Ruby: a, b = pair
来源：http://mgn.bbcook.cn

C#:   var (a, b) = pair;
来源：http://pnn.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://gvm.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://whr.smart0.xyz

PHP:  // 无重载
来源：http://tod.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yrm.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://bpe.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dti.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://yik.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://crd.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://krb.hysaishi.cn

================================================================================
来源：http://qwh.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://hvv.guowangkeji.top

================================================================================
来源：http://vfh.pycfn.com

[D01] 创建数组 / 列表
来源：http://tch.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hde.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jqd.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgi.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kdf.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yqi.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://cgh.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://nna.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://omq.yfazqb.com

[D02] 追加元素到末尾
来源：http://oci.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://afr.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tdz.hysaishi.cn

JS:   arr.push(4);
来源：http://bhh.hysaishi.cn

TS:   arr.push(4);
来源：http://uxq.yongpay.top

Java: list.add(4);
来源：http://trv.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://pip.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://gsu.redwolf501.top

C#:   list.Add(4);
来源：http://qec.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://bxh.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://lmu.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ksy.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dxm.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://qrq.tianlin.xyz

Java: list.add(0, 0);
来源：http://dam.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://syp.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pql.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://aud.yuanzhike.top

[D04] 删除元素
来源：http://dql.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://slf.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aef.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://klp.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://qqf.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wsa.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shm.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pvu.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tzx.shzxlz.cn

[D05] 访问与修改元素
来源：http://lhd.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ffn.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ctg.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sta.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://hlu.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://nmn.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://abx.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kxu.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wte.redwolf501.top

[D06] 数组长度
来源：http://kfd.feifeiyinyue.top

Py:   len(arr)
来源：http://ovh.fanxiaobao.xyz

PHP:  count($arr);
来源：http://vso.hnqzz.top

JS:   arr.length
来源：http://tye.meibo888.top

TS:   arr.length
来源：http://mmb.ydzc1.top

Java: list.size();
来源：http://ycn.jiagoushi.top

Go:   len(arr)
来源：http://tqx.redwolf501.top

Ruby: arr.length; arr.size
来源：http://sdn.nanxinkj.top

C#:   list.Count;
来源：http://qqf.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://lej.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ufj.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://cgp.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://wec.yongpay.top

TS:   arr.slice(1, 4);
来源：http://knd.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://wvu.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://mwc.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://yok.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://ztd.gaohongyu789.top

[D08] 合并两个数组
来源：http://wwe.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://kkb.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://rxb.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://grn.fzhhl.top

TS:   [...a, ...b];
来源：http://pag.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wfj.meibo888.top

Go:   append(a, b...)
来源：http://clo.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://ryd.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://vsm.cdnleiting.top

[D09] 排序（升序）
来源：http://frd.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://erh.shangyingyoupin.top

PHP:  sort($arr);
来源：http://zgc.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ebh.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sqb.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oyu.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cne.fzhhl.top

Ruby: arr.sort
来源：http://fiw.iojbl.cn

C#:   list.Sort();
来源：http://pga.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dlm.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qap.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whg.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbg.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgc.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lub.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rmx.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gcs.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tgt.jqgfzy.top

[D11] 反转数组
来源：http://nsh.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://pof.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://chl.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zof.svipenyu.cn

TS:   [...arr].reverse();
来源：http://mny.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://wgg.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://reu.nanxinkj.top

Ruby: arr.reverse
来源：http://cmq.xinyue.icu

C#:   list.Reverse();
来源：http://nap.52xcode.cn

[D12] 查找元素下标
来源：http://uwm.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://fni.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mxv.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://psh.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tae.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yja.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://sru.kuanghao11.cn

Ruby: arr.index(x)
来源：http://rvu.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://rpc.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://gox.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hyr.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ckl.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://lwj.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://qee.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vsg.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mjp.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fup.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jcy.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://ali.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dds.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lxr.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://ewm.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://hsm.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xss.haohaochexian.top

Go:   // 手写循环
来源：http://zke.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://uvo.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pej.meibo888.top

[D15] 去重
来源：http://ftq.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ueq.fengsongda.top

PHP:  array_unique($arr);
来源：http://zkf.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://ylt.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://bhg.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uua.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xff.hongshengwenyu.top

Ruby: arr.uniq
来源：http://btf.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://eca.nanxuanxn.top

[D16] 求和与平均值
来源：http://adg.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gvd.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://brr.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tct.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dmv.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uaq.yj20258.top

Go:   // 手写循环累加
来源：http://fqn.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dgd.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://qfg.gotoacloud.top

[D17] 最大值与最小值
来源：http://ujx.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://txu.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://ddz.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uib.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://gra.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jyj.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gnq.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://unx.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://mro.yj202588.top

[D18] 扁平化嵌套数组
来源：http://gsh.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qoh.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://zqp.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xdf.shanyushiyangtech.top

TS:   nested.flat();
来源：http://ssl.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xcp.cqqwz.cn

Go:   // 手写双层循环
来源：http://qat.ctjpmb.com

Ruby: nested.flatten
来源：http://fef.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xmz.nanxuanxn.top

[D19] 按字段分组
来源：http://hkg.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://frv.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kbx.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iwc.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kss.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nfz.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://lgu.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://idl.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yfo.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://aar.0kj1m.cn

Py:   Counter(arr)
来源：http://iub.aizwys.cn

PHP:  array_count_values($arr);
来源：http://pjx.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uln.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pps.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://azu.uphjek.com

Go:   // 手写 map[T]int
来源：http://stx.cucudq.cn

Ruby: arr.tally
来源：http://had.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bbr.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://jpq.c1oappe.top

Py:   x in arr
来源：http://mir.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://zyw.hcnkem.com

JS:   arr.includes(x)
来源：http://xxn.sxryk.cn

TS:   arr.includes(x)
来源：http://vtu.shzxlz.cn

Java: list.contains(x)
来源：http://vgp.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://qiu.fehbvm.com

Ruby: arr.include?(x)
来源：http://dko.hnxiangtu.top

C#:   list.Contains(x)
来源：http://ztl.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://hvv.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gwm.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://txd.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zec.jinqigfzy.top

TS:   [...arr];
来源：http://zqc.tanke756.top

Java: new ArrayList<>(list);
来源：http://jtt.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://pra.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://dqs.xuanzx.com

C#:   new List<int>(list);
来源：http://sle.shzxlz.cn

[D23] reduce 累积计算
来源：http://ihi.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lwv.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rbf.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://siu.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgz.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dfu.yj202588.top

Go:   // 手写循环
来源：http://huk.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pgy.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jfg.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://wkz.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cpn.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngj.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://arm.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://scc.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xor.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rxt.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vil.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fvk.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://srn.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aop.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ybj.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kfy.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xjw.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qzs.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://osn.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://utl.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dsb.nanxuanxn.top

[D26] 数组转字符串
来源：http://ezd.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://uxm.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://zjn.52xcode.cn

JS:   arr.join(", ")
来源：http://ass.xinyue.icu

TS:   arr.join(", ")
来源：http://ngp.chenzaomai.com

Java: String.join(", ", list)
来源：http://xuw.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://yxt.chenzaomai.com

Ruby: arr.join(", ")
来源：http://wqj.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://zfj.dashuyun.cn

================================================================================
来源：http://igv.xingfuxueyuan.xyz

E. 字符串处理
来源：http://fhc.yuanzhike.top

================================================================================
来源：http://jbg.jlsjyb.cn

[E01] 拼接字符串
来源：http://djy.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://opl.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hbs.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cog.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxv.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qss.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dgh.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ije.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qsl.yvedp.cn

[E02] 重复字符串
来源：http://zsx.iojbl.cn

Py:   "ab" * 3
来源：http://hfi.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://ztv.meibo888.top

JS:   "ab".repeat(3)
来源：http://egd.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://tsy.xylfe.cn

Java: "ab".repeat(3)
来源：http://zcy.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://nxz.fengsongda.top

Ruby: "ab" * 3
来源：http://xxo.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vbb.52xcode.cn

[E03] 截取子串
来源：http://sws.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fuu.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lml.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zzr.316326.xyz

TS:   s.slice(1, 4)
来源：http://qep.xylfe.cn

Java: s.substring(1, 4)
来源：http://eoz.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zir.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yyu.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://pyv.shangyingyoupin.top

[E04] 查找子串位置
来源：http://cbp.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://zep.redwolf501.top

PHP:  strpos($s, "x");
来源：http://bxp.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://osc.ydzc1.top

TS:   s.indexOf("x")
来源：http://jzd.daxiang520.top

Java: s.indexOf("x")
来源：http://kes.havefunace.top

Go:   strings.Index(s, "x")
来源：http://ejp.vqdsnc.cn

Ruby: s.index("x")
来源：http://amd.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://dhk.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://vgh.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bxt.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wub.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egd.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxr.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpf.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rvd.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njw.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jub.guowangkeji.top


<!-- 参考信息 -->