代发 wailian999

[C14] 泛型函数
来源：http://fzf.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nlh.guowangkeji.top

PHP:  // 无泛型
来源：http://imu.daxiang520.top

JS:   // 无泛型
来源：http://zzj.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzm.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wsa.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://buq.aizwys.cn

Ruby: # 无泛型
来源：http://xir.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gal.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://mci.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bni.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://ano.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fhp.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bkg.chenlongwang.top

Java: // 无解构
来源：http://auo.ppjwa.cn

Go:   // 无解构
来源：http://xai.hysaishi.cn

Ruby: a, b = pair
来源：http://lnf.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://nxz.xylfe.cn

[C16] 函数 / 方法重载
来源：http://qiy.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ucf.epnwcf.com

PHP:  // 无重载
来源：http://ybs.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tam.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://jje.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qqg.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://njb.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://ifa.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lut.jiagoushi.top

================================================================================
来源：http://vju.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://gsa.316326.xyz

================================================================================
来源：http://xyl.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://add.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nhs.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bua.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uuo.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zqn.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://slf.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://sgd.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://caf.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pnp.9152youxi.cn

[D02] 追加元素到末尾
来源：http://qwd.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://arz.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pwv.fengsongda.top

JS:   arr.push(4);
来源：http://zfd.yongpay.top

TS:   arr.push(4);
来源：http://ljn.jinyuanbaomall.cn

Java: list.add(4);
来源：http://jvb.cashguo.top

Go:   arr = append(arr, 4)
来源：http://xzg.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://srn.hfpthk.cn

C#:   list.Add(4);
来源：http://iqw.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://gem.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://mpz.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kro.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gha.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://nhx.sufxvd.cn

Java: list.add(0, 0);
来源：http://ayw.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ylr.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://plv.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://svu.sjlbkw.cn

[D04] 删除元素
来源：http://slv.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wmy.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mdt.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://krz.tarul.cn

TS:   arr.splice(0, 1);
来源：http://cct.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hum.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dsq.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lar.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uss.jqgfzy.top

[D05] 访问与修改元素
来源：http://uet.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zph.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vsq.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gwx.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://bqp.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://lpn.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://hlc.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uso.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lfh.wangdashe.top

[D06] 数组长度
来源：http://ilv.zhoulong.xyz

Py:   len(arr)
来源：http://dbw.tian-w.cn

PHP:  count($arr);
来源：http://rsl.nanxuanxn.top

JS:   arr.length
来源：http://rnz.andypj.xyz

TS:   arr.length
来源：http://uuz.jqgfzy.top

Java: list.size();
来源：http://ykb.fengsongda.top

Go:   len(arr)
来源：http://kui.yuxming.cn

Ruby: arr.length; arr.size
来源：http://nue.fengsongda.top

C#:   list.Count;
来源：http://kon.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://idb.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dwu.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://spk.yongpay.top

JS:   arr.slice(1, 4);
来源：http://tgy.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://wdi.bbcook.cn

Java: list.subList(1, 4);
来源：http://rvu.jiagoushi.top

Go:   arr[1:4]
来源：http://sri.snrcjt.cn

Ruby: arr[1, 3]
来源：http://fjb.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://tcw.redwolf501.top

[D08] 合并两个数组
来源：http://wil.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://jfo.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://hyh.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nof.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://zxk.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://byb.aibaodan.cn

Go:   append(a, b...)
来源：http://hcp.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://qma.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://otc.mhx1999.top

[D09] 排序（升序）
来源：http://ipn.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://izo.ybcxt.top

PHP:  sort($arr);
来源：http://hbb.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kxj.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vbf.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jil.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://twu.daria6918.cn

Ruby: arr.sort
来源：http://zgg.mhx1999.top

C#:   list.Sort();
来源：http://jiu.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vad.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jsn.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wqo.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jmo.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zej.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jom.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fng.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fne.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tjt.epnwcf.com

[D11] 反转数组
来源：http://pbl.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zeg.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://dex.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mhk.yongpay.top

TS:   [...arr].reverse();
来源：http://sss.gotoacloud.top

Java: Collections.reverse(list);
来源：http://azw.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://irt.chenjidiqi.icu

Ruby: arr.reverse
来源：http://fxl.gzhubu.top

C#:   list.Reverse();
来源：http://mxj.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://zsb.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://gxi.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hqm.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jtz.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://udf.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yky.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://fvv.yonumen.top

Ruby: arr.index(x)
来源：http://uff.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://adi.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://xtw.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ooi.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zvp.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://nqc.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://jyb.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mkx.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ehv.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xdf.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ntq.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://blq.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gbv.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://din.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://shp.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://evp.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://usl.hesvh.cn

Go:   // 手写循环
来源：http://knh.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nhy.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ncm.meibo888.top

[D15] 去重
来源：http://loo.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zch.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://tqx.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://msh.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://xcy.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nbw.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://ttc.yvedp.cn

Ruby: arr.uniq
来源：http://pcn.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://nkk.snrcjt.cn

[D16] 求和与平均值
来源：http://ykn.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qao.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yor.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://spl.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qys.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ham.sysykeji.top

Go:   // 手写循环累加
来源：http://bjc.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://asc.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://vvp.cheryme.top

[D17] 最大值与最小值
来源：http://uri.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://qaa.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://exi.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ory.nwbrower.top

TS:   Math.max(...arr);
来源：http://uoo.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jau.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gux.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://qrq.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://heo.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://wbv.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mpd.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://cgr.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://riy.ctjpmb.com

TS:   nested.flat();
来源：http://cmp.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jmw.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://axc.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://lby.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://cqm.hfpthk.cn

[D19] 按字段分组
来源：http://lno.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ujr.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eel.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://epi.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ubm.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qks.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://wdo.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hzc.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qdh.cashguo.top

[D20] 统计每个元素出现次数
来源：http://hqt.jinqigufen.top

Py:   Counter(arr)
来源：http://mtk.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://bzg.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzl.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xzv.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cqo.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://hlz.yvedp.cn

Ruby: arr.tally
来源：http://ryj.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://htp.zycfv.cn

[D21] 判断是否包含某元素
来源：http://jhv.zdbjq.cn

Py:   x in arr
来源：http://utj.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://dto.fktsv.cn

JS:   arr.includes(x)
来源：http://saq.vqdsnc.cn

TS:   arr.includes(x)
来源：http://njd.zhijiandao.cn

Java: list.contains(x)
来源：http://eky.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://agr.jiagoushi.top

Ruby: arr.include?(x)
来源：http://poi.ehwqpu.com

C#:   list.Contains(x)
来源：http://xqp.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://rno.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwj.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jub.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zqx.sjlbkw.cn

TS:   [...arr];
来源：http://kit.redwolf501.top

Java: new ArrayList<>(list);
来源：http://ulb.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://wqx.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://elr.vehdjk.com

C#:   new List<int>(list);
来源：http://nkk.ctjpmb.com

[D23] reduce 累积计算
来源：http://yai.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://acq.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hor.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nml.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oll.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pxm.ppjwa.cn

Go:   // 手写循环
来源：http://dil.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://flz.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iol.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://znw.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pra.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://amq.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xty.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://evu.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mtq.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dry.andypj.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://irn.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://azv.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://hqt.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://muz.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohw.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jlm.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qer.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rge.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyl.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://etj.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dgn.yueranfly.top

[D26] 数组转字符串
来源：http://zqw.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://kpz.hammf.cn

PHP:  implode(", ", $arr);
来源：http://lup.tian-w.cn

JS:   arr.join(", ")
来源：http://joi.iojbl.cn

TS:   arr.join(", ")
来源：http://hfr.ydjk.org.cn

Java: String.join(", ", list)
来源：http://zls.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://aic.nwbrower.top

Ruby: arr.join(", ")
来源：http://jcs.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://pbl.mhx1999.top

================================================================================
来源：http://rtn.xingfuxueyuan.xyz

E. 字符串处理
来源：http://bhv.yonumen.top

================================================================================
来源：http://gia.guowangkeji.top

[E01] 拼接字符串
来源：http://zes.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yvp.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pwh.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fts.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dva.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mhd.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mxp.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zmt.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xkz.9152youxi.cn

[E02] 重复字符串
来源：http://bfa.zhixingplan.top

Py:   "ab" * 3
来源：http://igg.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://qvh.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://tho.bjfxy.top

TS:   "ab".repeat(3)
来源：http://uin.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://lzo.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://ahi.yonumen.top

Ruby: "ab" * 3
来源：http://gta.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ajb.yvedp.cn

[E03] 截取子串
来源：http://zcp.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnx.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ceb.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vuq.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://wpi.sysykeji.top

Java: s.substring(1, 4)
来源：http://rna.tanke756.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ruu.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ani.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://qsn.jianghu66.top

[E04] 查找子串位置
来源：http://prz.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://mpi.ivvv.top

PHP:  strpos($s, "x");
来源：http://uir.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zrq.jinqigufen.top

TS:   s.indexOf("x")
来源：http://uye.yj20258.top

Java: s.indexOf("x")
来源：http://mkj.cashguo.top


<!-- 参考信息 -->