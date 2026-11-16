代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akw.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pae.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xkq.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xkn.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://azn.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://yno.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qlw.jiagoushi.top

[D02] 追加元素到末尾
来源：http://zsk.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://anq.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pez.chenlongwang.top

JS:   arr.push(4);
来源：http://tgs.sufxvd.cn

TS:   arr.push(4);
来源：http://dpg.vqdsnc.cn

Java: list.add(4);
来源：http://nxh.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://wsy.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://qaz.daria6918.cn

C#:   list.Add(4);
来源：http://yxq.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://gzk.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://xzw.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rau.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ryv.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://ckz.cqqwz.cn

Java: list.add(0, 0);
来源：http://bqh.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://not.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yrj.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://jkv.ppjwa.cn

[D04] 删除元素
来源：http://umv.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fng.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vwk.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cgt.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://hfl.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://phw.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lkf.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qfa.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pkn.pycfn.com

[D05] 访问与修改元素
来源：http://fow.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ttu.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ffz.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hhh.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://kaf.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://sbo.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ffu.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gkr.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ieb.hammf.cn

[D06] 数组长度
来源：http://abe.zdqjudy.top

Py:   len(arr)
来源：http://bcy.aibaodan.cn

PHP:  count($arr);
来源：http://wde.yuxming.cn

JS:   arr.length
来源：http://tin.chenzaomai.com

TS:   arr.length
来源：http://kxc.fehbvm.com

Java: list.size();
来源：http://gjm.iojbl.cn

Go:   len(arr)
来源：http://ltd.52xcode.cn

Ruby: arr.length; arr.size
来源：http://pjq.c1oappe.top

C#:   list.Count;
来源：http://buf.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://uom.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://buo.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tme.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://yjn.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://rwr.zhixingplan.top

Java: list.subList(1, 4);
来源：http://ktf.smart0.xyz

Go:   arr[1:4]
来源：http://mgo.nwbrower.top

Ruby: arr[1, 3]
来源：http://emi.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://nrf.zycfv.cn

[D08] 合并两个数组
来源：http://ast.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://vqv.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://zes.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mmc.cheryme.top

TS:   [...a, ...b];
来源：http://zwk.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pya.zycfv.cn

Go:   append(a, b...)
来源：http://zfq.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://eeq.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://bid.gzhubu.top

[D09] 排序（升序）
来源：http://vjy.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://zqe.shuidangran.top

PHP:  sort($arr);
来源：http://ksf.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hsm.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://alg.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uln.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fit.aizwys.cn

Ruby: arr.sort
来源：http://xwt.wangshuangyany.cn

C#:   list.Sort();
来源：http://svy.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nye.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://etk.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zkt.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uju.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nvl.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ccr.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dqq.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uwt.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dob.guowangkeji.top

[D11] 反转数组
来源：http://qoo.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://brj.bjfxy.top

PHP:  array_reverse($arr);
来源：http://owi.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://okq.yueranfly.top

TS:   [...arr].reverse();
来源：http://lak.yueranfly.top

Java: Collections.reverse(list);
来源：http://rse.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://qtg.sysykeji.top

Ruby: arr.reverse
来源：http://wmg.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://arc.haohaochexian.top

[D12] 查找元素下标
来源：http://sgn.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://fer.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://biz.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kbe.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cum.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dbg.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://cre.fehbvm.com

Ruby: arr.index(x)
来源：http://ypc.fktsv.cn

C#:   list.IndexOf(x);
来源：http://hik.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://txj.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zac.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tni.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://xxc.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://uyr.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kpw.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okz.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://gjm.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xhy.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://qce.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wjj.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ehx.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://kjf.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://yys.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kkt.c1oappe.top

Go:   // 手写循环
来源：http://qcc.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://dfq.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://azy.jinqigfzy.top

[D15] 去重
来源：http://cyl.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://miq.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://jrg.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://gdn.andypj.xyz

TS:   [...new Set(arr)]
来源：http://gqi.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djb.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://atv.0kj1m.cn

Ruby: arr.uniq
来源：http://gdy.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://bwj.shuidangran.top

[D16] 求和与平均值
来源：http://nae.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://del.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dgy.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pst.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qbz.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cig.gaohongyu789.top

Go:   // 手写循环累加
来源：http://jcv.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emq.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://dba.hnqzz.top

[D17] 最大值与最小值
来源：http://rkz.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://min.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://gzp.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://afg.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://fce.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ctg.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zzp.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://vds.uphjek.com

C#:   list.Max();  list.Min()
来源：http://rbi.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://ywz.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://azp.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://gfe.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vnn.aibaodan.cn

TS:   nested.flat();
来源：http://duj.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ail.guannengcc.top

Go:   // 手写双层循环
来源：http://jfv.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://ugw.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wlc.sjlbkw.cn

[D19] 按字段分组
来源：http://yzl.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uen.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ebi.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wtt.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ant.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wks.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://jap.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zaj.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cxf.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://trf.havefunace.top

Py:   Counter(arr)
来源：http://fws.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://qir.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wan.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://umj.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rum.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://uqq.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://jty.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rlm.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://wsl.hesvh.cn

Py:   x in arr
来源：http://rea.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://ikt.yvedp.cn

JS:   arr.includes(x)
来源：http://jog.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://qdy.fktsv.cn

Java: list.contains(x)
来源：http://jsy.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://ikm.cashguo.top

Ruby: arr.include?(x)
来源：http://blu.birdmap.top

C#:   list.Contains(x)
来源：http://goo.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://sui.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hqm.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qro.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://plo.gotoacloud.top

TS:   [...arr];
来源：http://jst.cheryme.top

Java: new ArrayList<>(list);
来源：http://zmv.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://mdn.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://urx.ppjwa.cn

C#:   new List<int>(list);
来源：http://diw.yonumen.top

[D23] reduce 累积计算
来源：http://xcd.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fgl.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://opw.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkz.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttx.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ijs.yvedp.cn

Go:   // 手写循环
来源：http://nlp.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://muw.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zgh.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://atd.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hng.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ekg.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rwb.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://opy.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://adn.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xcf.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qof.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vav.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://tmu.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cya.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yft.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jkp.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://awl.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ktn.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cnl.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uqc.nwbrower.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wya.tianlin.xyz

[D26] 数组转字符串
来源：http://arn.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://rwq.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://jke.ivvv.top

JS:   arr.join(", ")
来源：http://mez.jiagoushi.top

TS:   arr.join(", ")
来源：http://lky.hysaishi.cn

Java: String.join(", ", list)
来源：http://qyt.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://gdj.hfpthk.cn

Ruby: arr.join(", ")
来源：http://sww.hnqzz.top

C#:   string.Join(", ", list)
来源：http://jyv.ctjpmb.com

================================================================================
来源：http://mzm.epnwcf.com

E. 字符串处理
来源：http://bwn.52xcode.cn

================================================================================
来源：http://zwr.c1oappe.top

[E01] 拼接字符串
来源：http://jek.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ngw.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jfv.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://afi.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zno.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dpc.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ehs.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nzl.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfa.hammf.cn

[E02] 重复字符串
来源：http://lmy.ybcxt.top

Py:   "ab" * 3
来源：http://mts.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://wqx.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://yso.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://vqj.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://enh.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://wnk.jqgfzy.top

Ruby: "ab" * 3
来源：http://xos.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://efu.svipenyu.cn

[E03] 截取子串
来源：http://rfh.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ojk.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tuk.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rub.zycfv.cn

TS:   s.slice(1, 4)
来源：http://eec.jyoumei.cn

Java: s.substring(1, 4)
来源：http://hzv.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kbh.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://nvp.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://xvp.yonumen.top

[E04] 查找子串位置
来源：http://xth.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://szh.guannengcc.top

PHP:  strpos($s, "x");
来源：http://lmo.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jso.chenlongwang.top

TS:   s.indexOf("x")
来源：http://vxp.jianghu66.top

Java: s.indexOf("x")
来源：http://aej.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://alp.vqdsnc.cn

Ruby: s.index("x")
来源：http://aif.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://xda.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ueh.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qun.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tpg.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqi.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://rgb.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdr.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fnb.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ymx.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://faf.dianchejie.cn

[E06] 替换子串
来源：http://ijh.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vxi.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://xil.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyz.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://uhe.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ynb.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kzn.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yle.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://ezy.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://bol.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://raj.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pnq.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://omi.quarkkingdee.top

TS:   s.split(",")
来源：http://ylp.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xgc.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qcj.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://noh.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kjg.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://wiq.nanxinkj.top

Py:   ",".join(items)
来源：http://wzo.smart0.xyz


<!-- 参考信息 -->