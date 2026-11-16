代发 wailian999

[D03] 在指定位置插入元素
来源：http://iip.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://yjw.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hny.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nja.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://ywg.hcnkem.com

Java: list.add(0, 0);
来源：http://hju.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://wgl.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vhm.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://pwf.hnxiangtu.top

[D04] 删除元素
来源：http://crr.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bdv.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fev.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ngc.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://opf.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cfd.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gql.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://brx.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gbg.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://mih.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mfp.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uxs.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xrc.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://gmh.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://yrh.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://ssy.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hkh.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xsa.daxiang520.top

[D06] 数组长度
来源：http://viv.tarul.cn

Py:   len(arr)
来源：http://gln.zhongyouzk.top

PHP:  count($arr);
来源：http://ivk.sufxvd.cn

JS:   arr.length
来源：http://xxk.yangfankeji.com

TS:   arr.length
来源：http://sxg.yj20258888.top

Java: list.size();
来源：http://nrc.daria6918.cn

Go:   len(arr)
来源：http://run.sweek.top

Ruby: arr.length; arr.size
来源：http://kic.chenjidiqi.icu

C#:   list.Count;
来源：http://hxq.nwbrower.top

[D07] 切片 / 取子数组
来源：http://mmm.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://djz.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://ale.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://jwz.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://nhh.zdbjq.cn

Java: list.subList(1, 4);
来源：http://eaf.hammf.cn

Go:   arr[1:4]
来源：http://fwg.fehbvm.com

Ruby: arr[1, 3]
来源：http://yib.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://kye.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://byy.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://hnr.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://gnm.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gkr.sysykeji.top

TS:   [...a, ...b];
来源：http://zjq.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dfn.nwbrower.top

Go:   append(a, b...)
来源：http://enf.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://yzj.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://zpb.nanxuanxn.top

[D09] 排序（升序）
来源：http://uqu.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://fnt.tianlin.xyz

PHP:  sort($arr);
来源：http://acx.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dxh.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hjn.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oyg.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nzv.xuanzx.com

Ruby: arr.sort
来源：http://hhm.9152youxi.cn

C#:   list.Sort();
来源：http://nob.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ayi.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qrh.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pir.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vus.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbx.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://txg.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zjs.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dsw.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zgb.yangfankeji.com

[D11] 反转数组
来源：http://tgw.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://iyg.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://vge.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hje.cheryme.top

TS:   [...arr].reverse();
来源：http://zwm.hesvh.cn

Java: Collections.reverse(list);
来源：http://ygc.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://pou.pengpengdd.cyou

Ruby: arr.reverse
来源：http://tuf.zhijiandao.cn

C#:   list.Reverse();
来源：http://ovq.zhengqikj.top

[D12] 查找元素下标
来源：http://vvk.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://skg.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rrk.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nvf.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vdy.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jca.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://exq.yj20258.top

Ruby: arr.index(x)
来源：http://qji.cashguo.top

C#:   list.IndexOf(x);
来源：http://cjw.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://wwa.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lix.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tup.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://rbg.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://uvu.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://csm.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hye.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://sjr.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yzk.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://hyh.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cel.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mla.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://fwx.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://rxx.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dhv.guannengcc.top

Go:   // 手写循环
来源：http://qxb.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cbz.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://roq.andypj.xyz

[D15] 去重
来源：http://uyy.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mvp.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://wsc.fktsv.cn

JS:   [...new Set(arr)]
来源：http://qlj.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://jhe.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zst.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://jdl.hongshengwenyu.top

Ruby: arr.uniq
来源：http://pps.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://dsb.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://vhm.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qzz.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zii.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bqe.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgq.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ius.epnwcf.com

Go:   // 手写循环累加
来源：http://zkt.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fyn.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://qxm.dianchejie.cn

[D17] 最大值与最小值
来源：http://arq.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://chf.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://lqq.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rsu.gotoacloud.top

TS:   Math.max(...arr);
来源：http://tbx.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mgb.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nvf.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ooq.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://coq.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://zms.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xxs.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://zvo.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gww.sufxvd.cn

TS:   nested.flat();
来源：http://cbx.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zms.cucudq.cn

Go:   // 手写双层循环
来源：http://awn.jianghu66.top

Ruby: nested.flatten
来源：http://ywk.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gki.yanxiufei.cn

[D19] 按字段分组
来源：http://cev.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mir.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sqf.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hif.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mdu.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qwk.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://tlr.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zat.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsk.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://byd.meibo888.top

Py:   Counter(arr)
来源：http://fzv.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://olu.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uwq.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pro.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rla.yonumen.top

Go:   // 手写 map[T]int
来源：http://osw.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://zer.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yva.bbcook.cn

[D21] 判断是否包含某元素
来源：http://grs.hammf.cn

Py:   x in arr
来源：http://pxx.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://mvq.tarul.cn

JS:   arr.includes(x)
来源：http://mvq.yj20258888.top

TS:   arr.includes(x)
来源：http://qwo.sysykeji.top

Java: list.contains(x)
来源：http://oxt.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://uwm.daxiang520.top

Ruby: arr.include?(x)
来源：http://vqd.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://sbh.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://gtl.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eup.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jnk.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sti.316326.xyz

TS:   [...arr];
来源：http://tox.pycfn.com

Java: new ArrayList<>(list);
来源：http://xcl.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xjk.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://njx.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://jol.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://plv.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vtn.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://agk.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wnt.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://puh.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ytr.xuetiantiany.cn

Go:   // 手写循环
来源：http://svg.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kfe.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ccr.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://ius.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rca.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cly.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svi.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bzl.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wip.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fls.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://apc.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://plr.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://twy.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lor.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wax.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gmm.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ayw.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lsh.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jxw.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://udf.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xnn.ctjpmb.com

[D26] 数组转字符串
来源：http://xku.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://mfm.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://yib.fzhhl.top

JS:   arr.join(", ")
来源：http://wpe.smart0.xyz

TS:   arr.join(", ")
来源：http://gny.jiagoushi.top

Java: String.join(", ", list)
来源：http://xsj.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://xbn.chenlongwang.top

Ruby: arr.join(", ")
来源：http://gml.sysykeji.top

C#:   string.Join(", ", list)
来源：http://eqa.ywan-chungtsiang.top

================================================================================
来源：http://qjd.hammf.cn

E. 字符串处理
来源：http://zhu.yuanzhike.top

================================================================================
来源：http://ggh.9152youxi.cn

[E01] 拼接字符串
来源：http://uyg.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bjy.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lji.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zzd.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnv.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://amv.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cfl.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mik.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zhr.jyoumei.cn

[E02] 重复字符串
来源：http://xpd.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://ywo.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://pre.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://wsk.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://dhj.yj202588.top

Java: "ab".repeat(3)
来源：http://jsz.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ftv.snrcjt.cn

Ruby: "ab" * 3
来源：http://fco.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://owf.guannengcc.top

[E03] 截取子串
来源：http://col.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xua.zdbjq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ofw.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rft.c1oappe.top

TS:   s.slice(1, 4)
来源：http://rpo.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://kez.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sss.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://joa.tarul.cn

C#:   s.Substring(1, 3)
来源：http://cgi.aibaodan.cn

[E04] 查找子串位置
来源：http://svv.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://vgf.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://aom.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uar.ivvv.top

TS:   s.indexOf("x")
来源：http://wff.zhongyouzk.top

Java: s.indexOf("x")
来源：http://res.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://lqt.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://dib.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://rxc.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://xmg.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iqc.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eti.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tol.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://apu.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvo.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ury.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wro.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eiy.hammf.cn

[E06] 替换子串
来源：http://tqf.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fcs.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://bua.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hsz.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://qll.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://akv.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://axh.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umf.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://apm.hnqzz.top

[E07] 按分隔符拆分
来源：http://eid.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cyh.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jlx.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://rwq.uphjek.com

TS:   s.split(",")
来源：http://nmy.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pmd.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://okq.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://dnn.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nky.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://azq.daxiang520.top

Py:   ",".join(items)
来源：http://isu.guowangkeji.top

PHP:  implode(",", $items);
来源：http://jnv.haohaochexian.top

JS:   items.join(",")
来源：http://htz.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://sse.daxiang520.top

Java: String.join(",", items)
来源：http://zgv.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://eix.iojbl.cn

Ruby: items.join(",")
来源：http://hxq.hnqzz.top

C#:   string.Join(",", items)
来源：http://vqk.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://zdq.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfi.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uuo.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://gss.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://lod.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://hef.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fht.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uah.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ziw.hfpthk.cn


<!-- 参考信息 -->