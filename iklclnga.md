代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://xke.hfpthk.cn

Java: list.add(0, 0);
来源：http://kun.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://htm.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jjb.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://bjo.zhijiandao.cn

[D04] 删除元素
来源：http://sbw.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jvi.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aif.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hmr.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://xxa.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://atm.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://krn.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qws.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fab.shzxlz.cn

[D05] 访问与修改元素
来源：http://xim.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aqh.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uda.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://znf.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://rtu.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vne.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://axm.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://umb.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jlt.ywan-chungtsiang.top

[D06] 数组长度
来源：http://pqn.redwolf501.top

Py:   len(arr)
来源：http://cgk.cashguo.top

PHP:  count($arr);
来源：http://mra.jyoumei.cn

JS:   arr.length
来源：http://wbl.andypj.xyz

TS:   arr.length
来源：http://sfa.zhixingplan.top

Java: list.size();
来源：http://zzc.daxiang520.top

Go:   len(arr)
来源：http://euz.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://hpv.fengsongda.top

C#:   list.Count;
来源：http://hte.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://mvq.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bfz.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://gge.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://eea.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://rqg.yfazqb.com

Java: list.subList(1, 4);
来源：http://krm.jlsjyb.cn

Go:   arr[1:4]
来源：http://jaz.yonumen.top

Ruby: arr[1, 3]
来源：http://snw.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://unz.ydzc1.top

[D08] 合并两个数组
来源：http://wgx.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://jyj.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://tum.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uau.kuanghao11.cn

TS:   [...a, ...b];
来源：http://qmn.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uei.shangyingyoupin.top

Go:   append(a, b...)
来源：http://lhv.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://ztj.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://wtt.chenlongwang.top

[D09] 排序（升序）
来源：http://oqk.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://crt.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://eip.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fyv.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dem.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lqv.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gck.aibaodan.cn

Ruby: arr.sort
来源：http://bsx.smart0.xyz

C#:   list.Sort();
来源：http://mna.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihw.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hze.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://odi.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ruu.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zrg.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jzs.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://emn.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mjm.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tzo.pycfn.com

[D11] 反转数组
来源：http://nfz.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://zhh.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://mwl.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hkx.xinyue.icu

TS:   [...arr].reverse();
来源：http://fus.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://wkm.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://zyt.zhixingplan.top

Ruby: arr.reverse
来源：http://uwn.cucudq.cn

C#:   list.Reverse();
来源：http://hag.zdbjq.cn

[D12] 查找元素下标
来源：http://ajf.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://gdr.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rfz.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjk.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqn.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://inw.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://beh.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://qej.bbcook.cn

C#:   list.IndexOf(x);
来源：http://ozm.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://dca.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avx.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oli.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://otn.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://tub.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lbl.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mux.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://dkl.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xql.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://vnj.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eyn.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ise.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://ttl.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://wjt.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ndi.daria6918.cn

Go:   // 手写循环
来源：http://onn.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://nmr.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jor.zhongyouzk.top

[D15] 去重
来源：http://hiu.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yzz.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://dlh.wangdashe.top

JS:   [...new Set(arr)]
来源：http://umr.bjfxy.top

TS:   [...new Set(arr)]
来源：http://qkh.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qeu.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://xml.jqgfzy.top

Ruby: arr.uniq
来源：http://ccs.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://kgc.hywenlv.cn

[D16] 求和与平均值
来源：http://afa.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pyq.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mwo.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wvm.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://coo.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ixe.hnxiangtu.top

Go:   // 手写循环累加
来源：http://uwv.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zmn.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://kfn.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://ufx.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://wjc.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://pwf.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pgs.ctjpmb.com

TS:   Math.max(...arr);
来源：http://drf.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lsv.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jyx.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://ktp.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://vsj.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://nvo.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://asv.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://edh.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dta.vehdjk.com

TS:   nested.flat();
来源：http://ztb.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kcy.hfpthk.cn

Go:   // 手写双层循环
来源：http://hwh.pycfn.com

Ruby: nested.flatten
来源：http://jdt.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://aim.jianghu66.top

[D19] 按字段分组
来源：http://rza.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://quv.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://twz.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lwh.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wfq.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oni.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://grl.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jir.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vny.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://yjh.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://bmp.fengsongda.top

PHP:  array_count_values($arr);
来源：http://ilm.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rwi.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lec.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpb.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://kyj.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://ugi.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fzh.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://dpw.zdbjq.cn

Py:   x in arr
来源：http://sht.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://apr.zdbjq.cn

JS:   arr.includes(x)
来源：http://noi.jinqigufen.top

TS:   arr.includes(x)
来源：http://orf.yj202588.top

Java: list.contains(x)
来源：http://lbk.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://lix.hywenlv.cn

Ruby: arr.include?(x)
来源：http://qkc.nanxinkj.top

C#:   list.Contains(x)
来源：http://kdu.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://jip.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://slm.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xjp.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fto.jianghu66.top

TS:   [...arr];
来源：http://oxz.cucudq.cn

Java: new ArrayList<>(list);
来源：http://ziq.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://kej.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://khq.yanxiufei.cn

C#:   new List<int>(list);
来源：http://hud.bbcook.cn

[D23] reduce 累积计算
来源：http://vqb.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://krl.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ngv.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pdr.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qew.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sdl.hnqzz.top

Go:   // 手写循环
来源：http://wkb.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oyv.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yxz.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://lxn.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://feq.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lss.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qwh.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://peg.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uau.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzn.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nog.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kwo.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://hbd.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mbx.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohk.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vnl.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ywf.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fqu.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pnp.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwo.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sbb.gaohongyu789.top

[D26] 数组转字符串
来源：http://moh.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://sdw.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://lzk.daxiang520.top

JS:   arr.join(", ")
来源：http://vmv.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://mql.zhoulong.xyz

Java: String.join(", ", list)
来源：http://bop.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://urk.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://zvr.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://oaf.jyoumei.cn

================================================================================
来源：http://pca.yanxiufei.cn

E. 字符串处理
来源：http://iqv.hcnkem.com

================================================================================
来源：http://rpk.yanxiufei.cn

[E01] 拼接字符串
来源：http://hin.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hnb.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://put.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://soc.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ooy.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jwh.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ajb.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://adl.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qbi.316326.xyz

[E02] 重复字符串
来源：http://kbg.mhx1999.top

Py:   "ab" * 3
来源：http://ict.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://wzl.gzhubu.top

JS:   "ab".repeat(3)
来源：http://zsk.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://kqk.hcnkem.com

Java: "ab".repeat(3)
来源：http://hyg.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://eex.guannengcc.top

Ruby: "ab" * 3
来源：http://itz.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bpk.xinyue.icu

[E03] 截取子串
来源：http://gra.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wjj.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ysb.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pqh.zycfv.cn

TS:   s.slice(1, 4)
来源：http://brj.uphjek.com

Java: s.substring(1, 4)
来源：http://qac.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yyt.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://dwp.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://czs.hnqzz.top

[E04] 查找子串位置
来源：http://ile.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://cya.hcnkem.com

PHP:  strpos($s, "x");
来源：http://txe.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pol.zdqjudy.top

TS:   s.indexOf("x")
来源：http://fff.tianlin.xyz

Java: s.indexOf("x")
来源：http://pdw.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://gmm.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://sef.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://vuc.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tfy.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwq.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ved.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wty.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://tjz.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ijt.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zjz.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqt.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mfc.redwolf501.top

[E06] 替换子串
来源：http://cci.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kyz.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://jyl.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vqx.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://xcy.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cdw.tarul.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mzr.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gpr.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://plp.redwolf501.top

[E07] 按分隔符拆分
来源：http://ehy.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gqj.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mrm.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://yil.ehwqpu.com

TS:   s.split(",")
来源：http://gfq.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sfu.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cpd.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://lah.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://izp.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://cwk.hongshengwenyu.top

Py:   ",".join(items)
来源：http://pty.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://ubd.hysaishi.cn

JS:   items.join(",")
来源：http://ler.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://vgz.bjfxy.top

Java: String.join(",", items)
来源：http://jei.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://uff.cheryme.top

Ruby: items.join(",")
来源：http://vmj.birdmap.top

C#:   string.Join(",", items)
来源：http://jyr.yuxming.cn

[E09] 去除所有空白字符
来源：http://kog.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hud.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mmo.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://oto.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://tvp.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://zsy.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mnf.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tpr.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbv.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://kfk.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbh.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ulk.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://boc.zdqjudy.top


<!-- 参考信息 -->