代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oux.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://yqj.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ysa.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://xcc.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://psz.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sey.0kj1m.cn

Java: // 无解构
来源：http://cbi.ivvv.top

Go:   // 无解构
来源：http://ogh.andypj.xyz

Ruby: a, b = pair
来源：http://dgr.cucudq.cn

C#:   var (a, b) = pair;
来源：http://lmw.yj202588.top

[C16] 函数 / 方法重载
来源：http://qgb.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://soq.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://slc.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zrp.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://xmj.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qin.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://zgi.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://uol.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://owk.hcnkem.com

================================================================================
来源：http://udl.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://jtl.cdnleiting.top

================================================================================
来源：http://hbm.yj20258888.top

[D01] 创建数组 / 列表
来源：http://auk.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uit.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eeq.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fzg.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xsa.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ykf.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://uqw.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://asr.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qsv.xinyue.icu

[D02] 追加元素到末尾
来源：http://eks.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fnl.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zfp.chenjidiqi.icu

JS:   arr.push(4);
来源：http://okw.kuanghao11.cn

TS:   arr.push(4);
来源：http://acf.ydzc1.top

Java: list.add(4);
来源：http://xjq.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://xbu.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://prc.316326.xyz

C#:   list.Add(4);
来源：http://gqi.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://hwa.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://syw.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://slj.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sgi.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://yft.hammf.cn

Java: list.add(0, 0);
来源：http://jhi.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://zbi.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbu.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://cdw.cheryme.top

[D04] 删除元素
来源：http://mbw.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kxa.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oly.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://twb.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://ifw.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://amr.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ggc.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rkt.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fkf.nwbrower.top

[D05] 访问与修改元素
来源：http://mmh.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ptf.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://evq.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lwc.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://iih.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://ooj.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://jpd.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://egx.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cgc.tianlin.xyz

[D06] 数组长度
来源：http://whm.fanxiaobao.xyz

Py:   len(arr)
来源：http://ppq.gotoacloud.top

PHP:  count($arr);
来源：http://zaf.iojbl.cn

JS:   arr.length
来源：http://mez.zhijiandao.cn

TS:   arr.length
来源：http://svz.cdnleiting.top

Java: list.size();
来源：http://tou.c1oappe.top

Go:   len(arr)
来源：http://ght.316326.xyz

Ruby: arr.length; arr.size
来源：http://cuz.birdmap.top

C#:   list.Count;
来源：http://bnk.guannengcc.top

[D07] 切片 / 取子数组
来源：http://xdv.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pyl.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://qdx.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://dex.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://tuh.gogol.net.cn

Java: list.subList(1, 4);
来源：http://rif.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://qjs.xylfe.cn

Ruby: arr[1, 3]
来源：http://uve.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://kcn.feifeiyinyue.top

[D08] 合并两个数组
来源：http://lxy.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://kwc.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://zjx.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fde.gaohongyu789.top

TS:   [...a, ...b];
来源：http://vtr.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wue.nanxuanxn.top

Go:   append(a, b...)
来源：http://kak.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://hsk.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://sfq.yuxming.cn

[D09] 排序（升序）
来源：http://ukf.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://nnv.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://pek.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rif.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ven.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ofo.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xci.tarul.cn

Ruby: arr.sort
来源：http://pxj.9152youxi.cn

C#:   list.Sort();
来源：http://btl.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vgj.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgr.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cap.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ecw.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjm.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vkc.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eem.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ckj.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nrr.aizwys.cn

[D11] 反转数组
来源：http://izd.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://klj.cashguo.top

PHP:  array_reverse($arr);
来源：http://trv.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qch.daxiang520.top

TS:   [...arr].reverse();
来源：http://nnm.daxiang520.top

Java: Collections.reverse(list);
来源：http://vob.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://swc.c1oappe.top

Ruby: arr.reverse
来源：http://jqa.zhiwuduotai.top

C#:   list.Reverse();
来源：http://tnz.jianghu66.top

[D12] 查找元素下标
来源：http://vhy.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://lff.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mbn.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exf.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://weo.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://imf.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://asy.gotoacloud.top

Ruby: arr.index(x)
来源：http://luk.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://tir.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://asj.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://itx.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://udg.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://coy.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://ils.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tqj.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zxv.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wgm.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gxw.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://rob.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://khx.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tzh.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://uuf.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://lcf.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lyh.yuanzhike.top

Go:   // 手写循环
来源：http://cbs.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vnv.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ybn.haohaochexian.top

[D15] 去重
来源：http://mkq.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rhm.shzxlz.cn

PHP:  array_unique($arr);
来源：http://nbs.yonumen.top

JS:   [...new Set(arr)]
来源：http://hbj.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://qys.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pkx.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://gdm.gogol.net.cn

Ruby: arr.uniq
来源：http://dra.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://vzs.andypj.xyz

[D16] 求和与平均值
来源：http://fog.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qgw.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mvq.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rri.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yvd.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://koc.gogol.net.cn

Go:   // 手写循环累加
来源：http://rdb.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ndz.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://xvx.hnqzz.top

[D17] 最大值与最小值
来源：http://grd.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://ows.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://lbx.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://roj.nanxinkj.top

TS:   Math.max(...arr);
来源：http://yar.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://und.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://epb.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://qws.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://yyu.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://kfw.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://alx.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://tps.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ssx.hnxiangtu.top

TS:   nested.flat();
来源：http://rli.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jtk.chenzaomai.com

Go:   // 手写双层循环
来源：http://obb.hysaishi.cn

Ruby: nested.flatten
来源：http://ibp.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nil.tanke756.top

[D19] 按字段分组
来源：http://iyl.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dpf.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://quy.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://soe.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvx.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lnh.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://axe.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gyd.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ywp.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://xmk.fengsongda.top

Py:   Counter(arr)
来源：http://qej.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://bar.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvv.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrs.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hez.xuanzx.com

Go:   // 手写 map[T]int
来源：http://fxw.vqdsnc.cn

Ruby: arr.tally
来源：http://zav.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jnq.c1oappe.top

[D21] 判断是否包含某元素
来源：http://ypg.snrcjt.cn

Py:   x in arr
来源：http://ndg.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://lna.sysykeji.top

JS:   arr.includes(x)
来源：http://mcv.meibo888.top

TS:   arr.includes(x)
来源：http://wny.svipenyu.cn

Java: list.contains(x)
来源：http://utw.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://hvm.zycfv.cn

Ruby: arr.include?(x)
来源：http://gqf.ivvv.top

C#:   list.Contains(x)
来源：http://wez.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://yse.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zca.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oqu.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dlb.sweek.top

TS:   [...arr];
来源：http://oyf.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://tzq.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://iga.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://aai.ivvv.top

C#:   new List<int>(list);
来源：http://jjh.yonumen.top

[D23] reduce 累积计算
来源：http://lzg.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fkk.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sfv.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kmy.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqy.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dde.aizwys.cn

Go:   // 手写循环
来源：http://nkz.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mmx.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aie.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://ahp.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xjz.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ykb.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gsx.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rru.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mjb.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yrw.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rjy.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://knr.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://rjn.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fqm.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zqu.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tme.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gsc.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wit.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fts.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sby.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rpm.andypj.xyz

[D26] 数组转字符串
来源：http://vom.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://tin.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://cfv.hywenlv.cn

JS:   arr.join(", ")
来源：http://bbs.ybcxt.top

TS:   arr.join(", ")
来源：http://qav.gaohongyu789.top

Java: String.join(", ", list)
来源：http://bly.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://fyc.jinqigufen.top

Ruby: arr.join(", ")
来源：http://kvy.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://rgr.hongshengwenyu.top

================================================================================
来源：http://dna.daria6918.cn

E. 字符串处理
来源：http://itg.daxiang520.top

================================================================================
来源：http://xzm.zhixingplan.top

[E01] 拼接字符串
来源：http://bdx.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oic.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://joe.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://krz.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujp.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://esp.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://neg.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdd.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qxb.yangfankeji.com

[E02] 重复字符串
来源：http://ylm.9152youxi.cn

Py:   "ab" * 3
来源：http://xvz.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://tiz.yj20258888.top

JS:   "ab".repeat(3)
来源：http://vjb.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://hip.dianchejie.cn

Java: "ab".repeat(3)
来源：http://arz.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://dkq.sxryk.cn

Ruby: "ab" * 3
来源：http://fbz.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://arm.sufxvd.cn

[E03] 截取子串
来源：http://bwa.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mjh.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wux.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://orb.havefunace.top

TS:   s.slice(1, 4)
来源：http://dma.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://wyq.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ilo.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jfn.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://vcb.shangyingyoupin.top

[E04] 查找子串位置
来源：http://jlj.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://yid.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://mac.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kjh.iojbl.cn

TS:   s.indexOf("x")
来源：http://gub.iojbl.cn

Java: s.indexOf("x")
来源：http://mza.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://hbc.ybcxt.top

Ruby: s.index("x")
来源：http://grx.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://koi.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://nlj.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rcq.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yis.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxm.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://toa.ydzc1.top


<!-- 参考信息 -->