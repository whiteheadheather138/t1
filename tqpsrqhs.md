代发 wailian999

Ruby: a, b = pair
来源：http://jvy.316326.xyz

C#:   var (a, b) = pair;
来源：http://lpt.daria6918.cn

[C16] 函数 / 方法重载
来源：http://cve.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lks.yj20258.top

PHP:  // 无重载
来源：http://pff.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wsf.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://ocf.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fxj.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://gsz.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://zjx.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dtb.hysaishi.cn

================================================================================
来源：http://ciw.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://jex.gotoacloud.top

================================================================================
来源：http://jql.cheryme.top

[D01] 创建数组 / 列表
来源：http://thh.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gqd.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nrd.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nyq.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://knu.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vfo.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://lqq.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://obk.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qvn.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://rwx.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cdd.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ief.chenjidiqi.icu

JS:   arr.push(4);
来源：http://ajh.pycfn.com

TS:   arr.push(4);
来源：http://dni.ydzc1.top

Java: list.add(4);
来源：http://dge.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://ibt.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://jrp.sjlbkw.cn

C#:   list.Add(4);
来源：http://sqe.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://xxm.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://nil.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kgh.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mmt.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://cgu.quarkkingdee.top

Java: list.add(0, 0);
来源：http://pon.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://iua.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qay.316326.xyz

C#:   list.Insert(0, 0);
来源：http://fyn.vehdjk.com

[D04] 删除元素
来源：http://yko.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://weq.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://prr.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ymj.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://yuu.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqu.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://okt.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nzq.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lcl.yvedp.cn

[D05] 访问与修改元素
来源：http://lwk.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wio.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kgd.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://czc.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://ztv.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://bmh.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://aci.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fgk.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zhw.zhongyouzk.top

[D06] 数组长度
来源：http://osr.haohaochexian.top

Py:   len(arr)
来源：http://sjt.jqgufenzy.top

PHP:  count($arr);
来源：http://nel.gogol.net.cn

JS:   arr.length
来源：http://xbd.jinqigufen.top

TS:   arr.length
来源：http://tgo.c1oappe.top

Java: list.size();
来源：http://glv.fktsv.cn

Go:   len(arr)
来源：http://nra.ivvv.top

Ruby: arr.length; arr.size
来源：http://egl.jinghuilouyu.cn

C#:   list.Count;
来源：http://dfl.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://yxn.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sfz.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://gyi.yongpay.top

JS:   arr.slice(1, 4);
来源：http://rmr.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://jgn.vehdjk.com

Java: list.subList(1, 4);
来源：http://zkv.cqqwz.cn

Go:   arr[1:4]
来源：http://plz.uphjek.com

Ruby: arr[1, 3]
来源：http://lxp.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://vjg.cqqwz.cn

[D08] 合并两个数组
来源：http://xio.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://mwe.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://efi.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fsc.yfazqb.com

TS:   [...a, ...b];
来源：http://xor.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bfm.nanxinkj.top

Go:   append(a, b...)
来源：http://vfr.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://yie.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://nse.c1oappe.top

[D09] 排序（升序）
来源：http://hfo.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://gwl.sjlbkw.cn

PHP:  sort($arr);
来源：http://yow.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mns.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://seq.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yjc.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rpo.nanxinkj.top

Ruby: arr.sort
来源：http://ynz.yangfankeji.com

C#:   list.Sort();
来源：http://sxl.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://eti.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dms.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://chr.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhg.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nmh.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qsd.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lhl.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pdb.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://del.bbcook.cn

[D11] 反转数组
来源：http://qfa.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nrv.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://qyk.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gsz.hammf.cn

TS:   [...arr].reverse();
来源：http://qze.yj20258.top

Java: Collections.reverse(list);
来源：http://ngu.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://njl.chenzaomai.com

Ruby: arr.reverse
来源：http://xjy.hcnkem.com

C#:   list.Reverse();
来源：http://bng.uphjek.com

[D12] 查找元素下标
来源：http://ltv.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://rey.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ssk.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lzs.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://avg.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://scb.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://zlc.fzhhl.top

Ruby: arr.index(x)
来源：http://tcd.sysykeji.top

C#:   list.IndexOf(x);
来源：http://pea.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://twz.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ksx.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vbv.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://urm.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://mgx.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bqn.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bnt.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://dij.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://odq.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://ruf.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://txg.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rkh.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://dvg.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://uok.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nnh.chenzaomai.com

Go:   // 手写循环
来源：http://ily.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://fji.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://jsb.haohaochexian.top

[D15] 去重
来源：http://aaq.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyf.fehbvm.com

PHP:  array_unique($arr);
来源：http://xuj.ybcxt.top

JS:   [...new Set(arr)]
来源：http://zeu.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://ukf.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tko.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://fds.epnwcf.com

Ruby: arr.uniq
来源：http://wup.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://kkh.uphjek.com

[D16] 求和与平均值
来源：http://ekh.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ahj.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://boz.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mmk.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcg.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gyg.tarul.cn

Go:   // 手写循环累加
来源：http://fyt.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ddr.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://ytz.sweek.top

[D17] 最大值与最小值
来源：http://ffa.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://jay.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://yxk.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://irk.ppjwa.cn

TS:   Math.max(...arr);
来源：http://fyu.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iko.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ubr.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://dpw.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://ocr.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://yho.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://snb.hammf.cn

PHP:  array_merge(...$nested);
来源：http://dqs.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mbd.hfpthk.cn

TS:   nested.flat();
来源：http://pvu.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vxp.pycfn.com

Go:   // 手写双层循环
来源：http://gkp.gzhubu.top

Ruby: nested.flatten
来源：http://qvx.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://geg.jiagoushi.top

[D19] 按字段分组
来源：http://mzy.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://all.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hsn.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://njd.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fjj.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gip.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://xti.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpo.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ylm.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://gor.hcnkem.com

Py:   Counter(arr)
来源：http://jyu.hnqzz.top

PHP:  array_count_values($arr);
来源：http://lnk.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqg.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cnb.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wow.52xcode.cn

Go:   // 手写 map[T]int
来源：http://jiy.dianchejie.cn

Ruby: arr.tally
来源：http://nzy.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pmd.yfazqb.com

[D21] 判断是否包含某元素
来源：http://rnz.meibo888.top

Py:   x in arr
来源：http://ycq.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://tho.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://xmt.mhx1999.top

TS:   arr.includes(x)
来源：http://jnj.zhongyouzk.top

Java: list.contains(x)
来源：http://coz.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://tbs.daria6918.cn

Ruby: arr.include?(x)
来源：http://xvc.hywenlv.cn

C#:   list.Contains(x)
来源：http://ssd.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://bko.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xso.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vnt.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fnw.gzhubu.top

TS:   [...arr];
来源：http://jax.redwolf501.top

Java: new ArrayList<>(list);
来源：http://mvl.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://mdn.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://hhm.xziqi.cn

C#:   new List<int>(list);
来源：http://voa.iojbl.cn

[D23] reduce 累积计算
来源：http://cac.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kis.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hut.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mph.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozq.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://upn.shuidangran.top

Go:   // 手写循环
来源：http://hir.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ary.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ahg.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://fsz.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mtn.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rts.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tnc.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jgg.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zlz.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wnv.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cix.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fjm.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://aep.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://suq.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pft.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lpx.havefunace.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ahy.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vde.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hwf.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nsj.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eye.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://ovx.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://jtf.hammf.cn

PHP:  implode(", ", $arr);
来源：http://zja.yvedp.cn

JS:   arr.join(", ")
来源：http://wsy.yonumen.top

TS:   arr.join(", ")
来源：http://tqd.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://bpp.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://iip.sysykeji.top

Ruby: arr.join(", ")
来源：http://jxl.c1oappe.top

C#:   string.Join(", ", list)
来源：http://qgy.tian-w.cn

================================================================================
来源：http://ujq.epnwcf.com

E. 字符串处理
来源：http://uks.tianlin.xyz

================================================================================
来源：http://zca.hfpthk.cn

[E01] 拼接字符串
来源：http://nea.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://txc.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nma.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vme.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gcc.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://stt.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ueg.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zxb.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sqk.vqdsnc.cn

[E02] 重复字符串
来源：http://hog.hnqzz.top

Py:   "ab" * 3
来源：http://frp.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://sif.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://ifo.sysykeji.top

TS:   "ab".repeat(3)
来源：http://dvt.shzxlz.cn

Java: "ab".repeat(3)
来源：http://kcc.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://mjn.xuanzx.com

Ruby: "ab" * 3
来源：http://agg.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://che.xylfe.cn

[E03] 截取子串
来源：http://nii.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tvo.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cnf.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lfs.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://puz.daria6918.cn

Java: s.substring(1, 4)
来源：http://vvb.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dly.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bpz.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://ocj.cashguo.top

[E04] 查找子串位置
来源：http://rbd.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://yvi.iojbl.cn

PHP:  strpos($s, "x");
来源：http://dcn.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bnn.birdmap.top

TS:   s.indexOf("x")
来源：http://ijy.tianlin.xyz

Java: s.indexOf("x")
来源：http://axj.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://emm.ehwqpu.com

Ruby: s.index("x")
来源：http://zzj.hnqzz.top

C#:   s.IndexOf("x")
来源：http://swv.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://emq.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qlp.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qdl.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dsj.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://avc.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fqt.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ojz.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://efa.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wju.fengsongda.top

[E06] 替换子串
来源：http://ncf.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pxr.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://qoq.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nba.sufxvd.cn


<!-- 参考信息 -->