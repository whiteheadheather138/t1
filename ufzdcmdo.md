代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://las.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://obf.guowangkeji.top

Java: // 无解构
来源：http://dxc.daxiang520.top

Go:   // 无解构
来源：http://zjf.nanxuanxn.top

Ruby: a, b = pair
来源：http://udu.yongpay.top

C#:   var (a, b) = pair;
来源：http://zbc.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://skm.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ahu.hcnkem.com

PHP:  // 无重载
来源：http://rrl.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://udy.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://rkp.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eyd.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://lxc.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://gbi.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kqc.zhengqikj.top

================================================================================
来源：http://uon.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://brk.jinqigufen.top

================================================================================
来源：http://edn.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://vmv.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cjp.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pnz.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hqe.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://dyk.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gim.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ijv.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://xmf.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qtq.epnwcf.com

[D02] 追加元素到末尾
来源：http://jvo.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kxg.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sjn.cqqwz.cn

JS:   arr.push(4);
来源：http://hnm.chenzaomai.com

TS:   arr.push(4);
来源：http://kud.wangdashe.top

Java: list.add(4);
来源：http://cib.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://huv.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://asy.zycfv.cn

C#:   list.Add(4);
来源：http://nhm.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://siy.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://zyj.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bae.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ier.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://tkx.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://ooj.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ilz.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wlg.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://vil.zhijiandao.cn

[D04] 删除元素
来源：http://hef.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bkm.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eul.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hwy.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://ela.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ena.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://njv.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bdx.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jlg.ivvv.top

[D05] 访问与修改元素
来源：http://ens.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://itd.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nsq.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://unz.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://set.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://wdc.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://qjh.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://upc.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skh.shuidangran.top

[D06] 数组长度
来源：http://aky.jlsjyb.cn

Py:   len(arr)
来源：http://drz.hnqzz.top

PHP:  count($arr);
来源：http://ztc.hesvh.cn

JS:   arr.length
来源：http://pub.xuanzx.com

TS:   arr.length
来源：http://gox.vehdjk.com

Java: list.size();
来源：http://mxo.nwbrower.top

Go:   len(arr)
来源：http://jgh.xylfe.cn

Ruby: arr.length; arr.size
来源：http://noy.ydzc1.top

C#:   list.Count;
来源：http://hub.hnqzz.top

[D07] 切片 / 取子数组
来源：http://vsm.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uzq.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://atk.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://vkb.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://swo.xuanzx.com

Java: list.subList(1, 4);
来源：http://kef.daria6918.cn

Go:   arr[1:4]
来源：http://yqi.jqgfzy.top

Ruby: arr[1, 3]
来源：http://won.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://zkl.uphjek.com

[D08] 合并两个数组
来源：http://olh.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://quz.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://lcz.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uzp.shzxlz.cn

TS:   [...a, ...b];
来源：http://hqu.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://plp.havefunace.top

Go:   append(a, b...)
来源：http://wli.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://nip.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://ldn.bjfxy.top

[D09] 排序（升序）
来源：http://dkh.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://lrj.yueranfly.top

PHP:  sort($arr);
来源：http://mqs.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://apo.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eej.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jsx.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qbc.c1oappe.top

Ruby: arr.sort
来源：http://xwb.tanke756.top

C#:   list.Sort();
来源：http://fnr.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ads.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qxi.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vqw.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://exc.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sgc.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xph.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ilu.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wfv.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lka.jlsjyb.cn

[D11] 反转数组
来源：http://ukp.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://irn.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://nvf.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://clq.xylfe.cn

TS:   [...arr].reverse();
来源：http://oll.jqgfzy.top

Java: Collections.reverse(list);
来源：http://mzz.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://rvo.fengsongda.top

Ruby: arr.reverse
来源：http://wmj.9152youxi.cn

C#:   list.Reverse();
来源：http://xrj.zhijiandao.cn

[D12] 查找元素下标
来源：http://srv.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://ckh.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ked.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vlf.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zns.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://izp.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://bpm.yueranfly.top

Ruby: arr.index(x)
来源：http://kqp.tarul.cn

C#:   list.IndexOf(x);
来源：http://fqh.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://sqn.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://toc.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yyg.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://zay.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://qcz.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://owu.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gsu.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://tfk.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bat.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://vsa.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mvi.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ctq.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://ymr.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://eoj.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wgg.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://wyc.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://zve.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vyc.xuanzx.com

[D15] 去重
来源：http://nhq.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://izi.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://vvb.bjfxy.top

JS:   [...new Set(arr)]
来源：http://ryq.pycfn.com

TS:   [...new Set(arr)]
来源：http://tbf.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://clf.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://sfo.yonumen.top

Ruby: arr.uniq
来源：http://jke.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://udm.xuanzx.com

[D16] 求和与平均值
来源：http://pvn.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://acj.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aay.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgu.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ney.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywd.gogol.net.cn

Go:   // 手写循环累加
来源：http://roy.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dqh.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://ugm.haohaochexian.top

[D17] 最大值与最小值
来源：http://qxc.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://aoz.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://xaj.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cuv.wangdashe.top

TS:   Math.max(...arr);
来源：http://tfa.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://biy.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jby.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://qfy.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://cqo.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://ivg.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rkk.ivvv.top

PHP:  array_merge(...$nested);
来源：http://vay.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hpb.cqqwz.cn

TS:   nested.flat();
来源：http://goa.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cbt.fzhhl.top

Go:   // 手写双层循环
来源：http://nbt.snrcjt.cn

Ruby: nested.flatten
来源：http://qby.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xww.fanxiaobao.xyz

[D19] 按字段分组
来源：http://cof.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://are.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fhd.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ozk.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wbd.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mce.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://yut.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kts.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jks.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://nno.zhongyouzk.top

Py:   Counter(arr)
来源：http://zie.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://kqd.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gem.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jla.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lzd.havefunace.top

Go:   // 手写 map[T]int
来源：http://sdw.meibo888.top

Ruby: arr.tally
来源：http://jpl.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mpw.hesvh.cn

[D21] 判断是否包含某元素
来源：http://qdy.yanxiufei.cn

Py:   x in arr
来源：http://xhz.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://iho.epnwcf.com

JS:   arr.includes(x)
来源：http://itz.birdmap.top

TS:   arr.includes(x)
来源：http://bif.52xcode.cn

Java: list.contains(x)
来源：http://acf.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://ury.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://dib.jqgfzy.top

C#:   list.Contains(x)
来源：http://wqq.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://zfq.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sxe.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zka.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jnf.yfazqb.com

TS:   [...arr];
来源：http://rre.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://zgd.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mpw.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://gcw.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://gjo.yj20258888.top

[D23] reduce 累积计算
来源：http://kic.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ldq.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qmt.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ize.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://twy.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jaw.hcnkem.com

Go:   // 手写循环
来源：http://kvz.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pnl.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lgn.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://tqg.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dkw.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fnh.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyo.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xrv.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ukg.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ocy.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qrc.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uhj.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://nxa.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qxu.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yay.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ejf.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hco.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rai.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://utx.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dgh.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yxs.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://tgk.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://jpg.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://frn.haohaochexian.top

JS:   arr.join(", ")
来源：http://zxn.daxiang520.top

TS:   arr.join(", ")
来源：http://gvw.sjlbkw.cn

Java: String.join(", ", list)
来源：http://fsw.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://qnb.gzhubu.top

Ruby: arr.join(", ")
来源：http://ojg.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://zss.wangshuangyany.cn

================================================================================
来源：http://yyc.havefunace.top

E. 字符串处理
来源：http://qsq.shangyingyoupin.top

================================================================================
来源：http://pvq.zhijiandao.cn

[E01] 拼接字符串
来源：http://sqs.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wkz.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zqo.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nhf.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fhk.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lpl.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dcb.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hrh.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pbi.jinqigfzy.top

[E02] 重复字符串
来源：http://ykb.ppjwa.cn

Py:   "ab" * 3
来源：http://dvm.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://vvt.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://rfh.tanke756.top

TS:   "ab".repeat(3)
来源：http://cvk.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://sia.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://cbs.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://ucw.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wex.haohaochexian.top

[E03] 截取子串
来源：http://aml.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ixl.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nwp.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://okb.yvedp.cn

TS:   s.slice(1, 4)
来源：http://vvk.jinqigufen.top

Java: s.substring(1, 4)
来源：http://nhl.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uoy.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://phb.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://emg.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://ecl.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://vrb.fehbvm.com

PHP:  strpos($s, "x");
来源：http://csh.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dyz.ydzc1.top

TS:   s.indexOf("x")
来源：http://pad.hesvh.cn

Java: s.indexOf("x")
来源：http://doe.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://bgl.wangshuangyany.cn

Ruby: s.index("x")
来源：http://cub.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://siz.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eku.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oru.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nns.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fhi.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wvo.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vcq.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ewx.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://isw.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dzq.yj202588.top


<!-- 参考信息 -->