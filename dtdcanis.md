代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jbg.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://tma.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://urf.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://ybn.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ded.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wfv.hcnkem.com

Java: // 无解构
来源：http://lwx.mhx1999.top

Go:   // 无解构
来源：http://nyu.haohaochexian.top

Ruby: a, b = pair
来源：http://cri.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://sjs.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://qoa.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wjo.9152youxi.cn

PHP:  // 无重载
来源：http://nui.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdj.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://hio.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sio.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://nnr.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://jat.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gts.gzhubu.top

================================================================================
来源：http://lkv.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://syh.daria6918.cn

================================================================================
来源：http://cvb.yongpay.top

[D01] 创建数组 / 列表
来源：http://jsh.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://utm.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qjt.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ull.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tpv.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgy.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://vog.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://mok.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://suh.hcnkem.com

[D02] 追加元素到末尾
来源：http://aoh.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jvx.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://toc.ivvv.top

JS:   arr.push(4);
来源：http://eie.shuidangran.top

TS:   arr.push(4);
来源：http://knt.zhijiandao.cn

Java: list.add(4);
来源：http://xhf.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://pgb.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://neg.gogol.net.cn

C#:   list.Add(4);
来源：http://mgo.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://ohx.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://sij.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gvc.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tdv.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://plb.guannengcc.top

Java: list.add(0, 0);
来源：http://fiv.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ljy.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qua.ivvv.top

C#:   list.Insert(0, 0);
来源：http://rfw.ydjk.org.cn

[D04] 删除元素
来源：http://ibs.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rjq.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dhe.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pka.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://gww.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vtf.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vtf.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqe.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rwq.haohaochexian.top

[D05] 访问与修改元素
来源：http://jfk.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gzv.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aib.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nup.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://gix.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://stj.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://kfy.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ehl.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ykf.smart0.xyz

[D06] 数组长度
来源：http://pqt.ydzc1.top

Py:   len(arr)
来源：http://osm.nanxinkj.top

PHP:  count($arr);
来源：http://njs.hfpthk.cn

JS:   arr.length
来源：http://mnv.fanxiaobao.xyz

TS:   arr.length
来源：http://pix.zhengqikj.top

Java: list.size();
来源：http://aal.wangdashe.top

Go:   len(arr)
来源：http://lbr.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://lmw.dianchejie.cn

C#:   list.Count;
来源：http://uih.aizwys.cn

[D07] 切片 / 取子数组
来源：http://ljv.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://evd.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wcz.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://rxk.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://wrz.fzhhl.top

Java: list.subList(1, 4);
来源：http://gsf.vqdsnc.cn

Go:   arr[1:4]
来源：http://kxw.316326.xyz

Ruby: arr[1, 3]
来源：http://kuh.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://fla.tarul.cn

[D08] 合并两个数组
来源：http://xcs.sweek.top

Py:   a + b;  a.extend(b)
来源：http://lfz.316326.xyz

PHP:  array_merge($a, $b);
来源：http://anm.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://frn.yangfankeji.com

TS:   [...a, ...b];
来源：http://wom.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://idh.snrcjt.cn

Go:   append(a, b...)
来源：http://pre.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://ino.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://odk.yuanzhike.top

[D09] 排序（升序）
来源：http://jlx.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://bfc.svipenyu.cn

PHP:  sort($arr);
来源：http://uss.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nep.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aan.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rln.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://owy.hesvh.cn

Ruby: arr.sort
来源：http://jnf.zdbjq.cn

C#:   list.Sort();
来源：http://qug.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ayo.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://owb.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qwi.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgc.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryn.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xsh.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ohs.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lbl.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gfx.jianghu66.top

[D11] 反转数组
来源：http://kut.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lmd.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://mnr.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rep.iojbl.cn

TS:   [...arr].reverse();
来源：http://gdt.yuxming.cn

Java: Collections.reverse(list);
来源：http://ovl.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://kiq.uphjek.com

Ruby: arr.reverse
来源：http://aqs.cheryme.top

C#:   list.Reverse();
来源：http://dnl.xziqi.cn

[D12] 查找元素下标
来源：http://eum.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://wnv.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://etx.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iiq.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eam.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://juz.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://xur.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://shp.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://kld.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://jaz.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ebx.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rnf.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://opo.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://qxw.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bpf.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpn.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tqj.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bvw.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://pcy.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fxo.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cda.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://zkv.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://xwt.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ghl.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://qim.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://djw.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rrn.aibaodan.cn

[D15] 去重
来源：http://rbh.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tmc.hcnkem.com

PHP:  array_unique($arr);
来源：http://ftd.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://pup.wangdashe.top

TS:   [...new Set(arr)]
来源：http://ftg.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fof.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://uex.uphjek.com

Ruby: arr.uniq
来源：http://juw.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://dcc.zhongyouzk.top

[D16] 求和与平均值
来源：http://ygm.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nsr.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tzc.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tje.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuo.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hdh.nwbrower.top

Go:   // 手写循环累加
来源：http://joh.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mva.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://mjq.shuidangran.top

[D17] 最大值与最小值
来源：http://hax.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://iyp.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://ugn.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://afd.zhengqikj.top

TS:   Math.max(...arr);
来源：http://ytm.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gwo.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vgr.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://ebi.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://svl.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://anj.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://knf.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://xxm.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iko.chenlongwang.top

TS:   nested.flat();
来源：http://dxv.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bse.vqdsnc.cn

Go:   // 手写双层循环
来源：http://ujn.jinqigfzy.top

Ruby: nested.flatten
来源：http://xva.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ung.hcnkem.com

[D19] 按字段分组
来源：http://nsr.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xum.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://abi.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kmi.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hag.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vob.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://zen.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ogo.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sfw.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://umf.smart0.xyz

Py:   Counter(arr)
来源：http://tpo.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://qdk.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wqg.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gra.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wtl.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://xbo.ctjpmb.com

Ruby: arr.tally
来源：http://kbz.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zzs.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://bxm.smart0.xyz

Py:   x in arr
来源：http://elf.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://nrj.daxiang520.top

JS:   arr.includes(x)
来源：http://ogh.tian-w.cn

TS:   arr.includes(x)
来源：http://xls.iojbl.cn

Java: list.contains(x)
来源：http://bxk.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://mvb.daxiang520.top

Ruby: arr.include?(x)
来源：http://kij.daxiang520.top

C#:   list.Contains(x)
来源：http://rgx.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://kjs.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ihi.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kks.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://srt.mhx1999.top

TS:   [...arr];
来源：http://eab.sweek.top

Java: new ArrayList<>(list);
来源：http://szj.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://kmy.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://pbo.ydzc1.top

C#:   new List<int>(list);
来源：http://meo.zhengqikj.top

[D23] reduce 累积计算
来源：http://zxm.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wlj.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hgr.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ybb.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uub.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://egt.cdnleiting.top

Go:   // 手写循环
来源：http://mkj.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lwt.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://huc.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://hyh.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://suk.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lbj.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aoy.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ckf.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fty.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ade.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wmb.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tgn.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://zfl.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vbr.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yeo.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jux.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zds.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wyz.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zfw.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eix.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ugy.shuidangran.top

[D26] 数组转字符串
来源：http://dty.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://tjs.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://buh.bjfxy.top

JS:   arr.join(", ")
来源：http://cbc.xylfe.cn

TS:   arr.join(", ")
来源：http://eks.gzhubu.top

Java: String.join(", ", list)
来源：http://wak.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://swx.ivvv.top

Ruby: arr.join(", ")
来源：http://pxz.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://eth.svipenyu.cn

================================================================================
来源：http://sct.fengsongda.top

E. 字符串处理
来源：http://cly.aibaodan.cn

================================================================================
来源：http://mvt.zdbjq.cn

[E01] 拼接字符串
来源：http://akn.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bvd.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ctz.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnj.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppp.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ulw.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dnm.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://srt.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rsw.dianchejie.cn

[E02] 重复字符串
来源：http://ogu.hcnkem.com

Py:   "ab" * 3
来源：http://rnt.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://xii.meibo888.top

JS:   "ab".repeat(3)
来源：http://rts.hnqzz.top

TS:   "ab".repeat(3)
来源：http://emz.haohaochexian.top

Java: "ab".repeat(3)
来源：http://xws.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://yba.yonumen.top

Ruby: "ab" * 3
来源：http://buk.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zth.xinyue.icu

[E03] 截取子串
来源：http://kfl.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wdn.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zti.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sat.mhx1999.top

TS:   s.slice(1, 4)
来源：http://ftz.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://jgf.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pun.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://imn.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://efp.cqqwz.cn

[E04] 查找子串位置
来源：http://qzl.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://vfs.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://mhk.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eif.hnqzz.top

TS:   s.indexOf("x")
来源：http://zms.vqdsnc.cn

Java: s.indexOf("x")
来源：http://kte.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://akr.dashuyun.cn

Ruby: s.index("x")
来源：http://pkg.aizwys.cn

C#:   s.IndexOf("x")
来源：http://wsp.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vho.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bjy.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kwf.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://opp.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ouz.smart0.xyz


<!-- 参考信息 -->