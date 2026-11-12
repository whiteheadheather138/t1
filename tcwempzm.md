代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baz.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xrr.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zhf.kuanghao11.cn

Ruby: # 无泛型
来源：http://tzt.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hbl.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://nfy.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pot.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://vta.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uvf.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://raa.ctjpmb.com

Java: // 无解构
来源：http://ewd.zhengqikj.top

Go:   // 无解构
来源：http://xlh.tian-w.cn

Ruby: a, b = pair
来源：http://znq.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://wpo.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://usx.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fyv.aizwys.cn

PHP:  // 无重载
来源：http://vug.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ycg.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://zdd.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qup.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://bkn.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://bdc.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xcn.fzhhl.top

================================================================================
来源：http://qgy.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://sgx.nanxuanxn.top

================================================================================
来源：http://rrt.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://jhr.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dad.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wrp.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://myi.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://org.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hpx.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://wzz.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://xzv.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zcd.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://yja.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kbl.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xwx.yangfankeji.com

JS:   arr.push(4);
来源：http://yab.nanxuanxn.top

TS:   arr.push(4);
来源：http://wbb.shangyingyoupin.top

Java: list.add(4);
来源：http://uwq.tarul.cn

Go:   arr = append(arr, 4)
来源：http://uxy.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://vuw.gzhubu.top

C#:   list.Add(4);
来源：http://yjh.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://bpf.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://qrj.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://slf.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dgd.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://ayg.cdnleiting.top

Java: list.add(0, 0);
来源：http://piu.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://pdg.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://txc.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://biv.yj20258.top

[D04] 删除元素
来源：http://pkw.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gdt.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://utg.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nzm.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://gyr.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hpu.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hmu.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://prt.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cdw.xziqi.cn

[D05] 访问与修改元素
来源：http://spv.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wkb.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nnk.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aiu.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://zew.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://rnd.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://brj.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rnr.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qno.jinqigufen.top

[D06] 数组长度
来源：http://lya.fzhhl.top

Py:   len(arr)
来源：http://ksa.ybcxt.top

PHP:  count($arr);
来源：http://emg.yanxiufei.cn

JS:   arr.length
来源：http://itk.nwbrower.top

TS:   arr.length
来源：http://nau.fktsv.cn

Java: list.size();
来源：http://fuz.dianchejie.cn

Go:   len(arr)
来源：http://abf.redwolf501.top

Ruby: arr.length; arr.size
来源：http://hby.yonumen.top

C#:   list.Count;
来源：http://zid.iojbl.cn

[D07] 切片 / 取子数组
来源：http://wiy.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cip.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://amh.tarul.cn

JS:   arr.slice(1, 4);
来源：http://zje.316326.xyz

TS:   arr.slice(1, 4);
来源：http://cwc.vehdjk.com

Java: list.subList(1, 4);
来源：http://wea.jiagoushi.top

Go:   arr[1:4]
来源：http://aoh.zdbjq.cn

Ruby: arr[1, 3]
来源：http://knx.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://lex.tanke756.top

[D08] 合并两个数组
来源：http://yke.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://mmv.sweek.top

PHP:  array_merge($a, $b);
来源：http://sct.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ezs.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://aev.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kkd.ehwqpu.com

Go:   append(a, b...)
来源：http://twq.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://lbo.sweek.top

C#:   a.Concat(b).ToList()
来源：http://enx.tarul.cn

[D09] 排序（升序）
来源：http://opp.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://jba.daxiang520.top

PHP:  sort($arr);
来源：http://ffm.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bwb.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgh.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wwn.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bsd.mhx1999.top

Ruby: arr.sort
来源：http://clv.zhongyouzk.top

C#:   list.Sort();
来源：http://hgk.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfc.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvc.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nhw.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhl.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvr.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oqv.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dco.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://giu.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mur.316326.xyz

[D11] 反转数组
来源：http://wmi.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://cfz.sysykeji.top

PHP:  array_reverse($arr);
来源：http://zla.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xzs.uphjek.com

TS:   [...arr].reverse();
来源：http://wfr.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://oqa.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://rym.quarkkingdee.top

Ruby: arr.reverse
来源：http://clc.smart0.xyz

C#:   list.Reverse();
来源：http://atb.jlsjyb.cn

[D12] 查找元素下标
来源：http://dlq.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://jci.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ake.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecq.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxw.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wjl.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://coa.zdbjq.cn

Ruby: arr.index(x)
来源：http://yeu.cucudq.cn

C#:   list.IndexOf(x);
来源：http://gkz.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://hmn.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bef.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ssa.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://urk.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://dio.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://giw.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vag.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://lqi.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lkp.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://crh.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nen.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yml.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://pes.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://teg.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mac.sweek.top

Go:   // 手写循环
来源：http://wua.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uag.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zma.gogol.net.cn

[D15] 去重
来源：http://llp.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pfl.ydzc1.top

PHP:  array_unique($arr);
来源：http://add.mhx1999.top

JS:   [...new Set(arr)]
来源：http://pre.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://edy.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://drf.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://yzc.zhongyouzk.top

Ruby: arr.uniq
来源：http://tgb.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://aqf.xuetiantiany.cn

[D16] 求和与平均值
来源：http://aio.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hqy.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ewi.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpu.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xno.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uir.zhijiandao.cn

Go:   // 手写循环累加
来源：http://swf.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aip.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://lam.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://hbi.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://pkd.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://upw.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://die.nwbrower.top

TS:   Math.max(...arr);
来源：http://xrb.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://emf.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://elz.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://oua.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://jfa.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://daq.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayr.havefunace.top

PHP:  array_merge(...$nested);
来源：http://lzk.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pgi.316326.xyz

TS:   nested.flat();
来源：http://uvb.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rsi.tianlin.xyz

Go:   // 手写双层循环
来源：http://dbb.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://gzj.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://adb.sjlbkw.cn

[D19] 按字段分组
来源：http://oeq.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iwm.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmf.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uin.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ipq.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eoi.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://yom.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vsg.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bhp.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://pnx.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://efb.xuanzx.com

PHP:  array_count_values($arr);
来源：http://ucq.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ncz.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vnt.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ntc.havefunace.top

Go:   // 手写 map[T]int
来源：http://xxo.chenlongwang.top

Ruby: arr.tally
来源：http://yxw.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://opg.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://teb.gaohongyu789.top

Py:   x in arr
来源：http://ifi.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://afj.yonumen.top

JS:   arr.includes(x)
来源：http://syb.hammf.cn

TS:   arr.includes(x)
来源：http://ync.vehdjk.com

Java: list.contains(x)
来源：http://ivq.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://nxw.shzxlz.cn

Ruby: arr.include?(x)
来源：http://icb.ydzc1.top

C#:   list.Contains(x)
来源：http://qaf.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://sqr.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kus.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://enb.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ipk.zhongyouzk.top

TS:   [...arr];
来源：http://zzs.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://cly.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://qmt.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://fhc.yuanzhike.top

C#:   new List<int>(list);
来源：http://ndw.gotoacloud.top

[D23] reduce 累积计算
来源：http://thj.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rhp.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cwe.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hko.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfm.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iss.vqdsnc.cn

Go:   // 手写循环
来源：http://rho.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://czq.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://znt.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://hhf.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ryp.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yub.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpj.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://btr.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nru.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ihj.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eku.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eqj.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://osw.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ilf.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lff.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yru.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ipa.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ngl.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gkh.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://faw.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bog.zhengqikj.top

[D26] 数组转字符串
来源：http://koo.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://wmj.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://vsh.gzhubu.top

JS:   arr.join(", ")
来源：http://qpb.redwolf501.top

TS:   arr.join(", ")
来源：http://duu.ydjk.org.cn

Java: String.join(", ", list)
来源：http://zzv.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://jhj.ctjpmb.com

Ruby: arr.join(", ")
来源：http://can.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://ban.sysykeji.top

================================================================================
来源：http://zaw.haohaochexian.top

E. 字符串处理
来源：http://tyt.cheryme.top

================================================================================
来源：http://szd.pycfn.com

[E01] 拼接字符串
来源：http://zur.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fpj.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mvn.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jui.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://elz.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kdg.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yvb.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nmz.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oor.zhongyouzk.top

[E02] 重复字符串
来源：http://sne.zycfv.cn

Py:   "ab" * 3
来源：http://man.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://iyr.hesvh.cn

JS:   "ab".repeat(3)
来源：http://kwl.nwbrower.top

TS:   "ab".repeat(3)
来源：http://icd.jianghu66.top

Java: "ab".repeat(3)
来源：http://wlc.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://dzn.epnwcf.com

Ruby: "ab" * 3
来源：http://kcg.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ofk.bjfxy.top

[E03] 截取子串
来源：http://ize.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://atr.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://awx.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tcd.mhx1999.top

TS:   s.slice(1, 4)
来源：http://qam.xinyue.icu

Java: s.substring(1, 4)
来源：http://ofs.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aak.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ncl.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://bgh.0kj1m.cn

[E04] 查找子串位置
来源：http://lvh.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://zqe.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://goa.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qjt.vehdjk.com

TS:   s.indexOf("x")
来源：http://mtx.ppjwa.cn

Java: s.indexOf("x")
来源：http://mlt.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://wdo.hysaishi.cn

Ruby: s.index("x")
来源：http://xvm.daria6918.cn

C#:   s.IndexOf("x")
来源：http://xyk.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqc.jqgfzy.top


<!-- 参考信息 -->