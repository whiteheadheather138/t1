代发 wailian999

Java: list.add(4);
来源：http://zmi.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://ehp.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://nfb.yuxming.cn

C#:   list.Add(4);
来源：http://pcv.meibo888.top

[D03] 在指定位置插入元素
来源：http://zfo.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://guj.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bdo.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ijv.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://rms.yvedp.cn

Java: list.add(0, 0);
来源：http://oik.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xww.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qng.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://imz.jyoumei.cn

[D04] 删除元素
来源：http://bzb.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xjj.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://emw.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vvm.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://nrc.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksw.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcj.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ehr.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jtp.c1oappe.top

[D05] 访问与修改元素
来源：http://azi.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qjg.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://axp.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ocd.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://rnp.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://xhw.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://oae.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mei.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mel.sjlbkw.cn

[D06] 数组长度
来源：http://aqh.svipenyu.cn

Py:   len(arr)
来源：http://cqe.redwolf501.top

PHP:  count($arr);
来源：http://jdj.xziqi.cn

JS:   arr.length
来源：http://uiz.pycfn.com

TS:   arr.length
来源：http://jvh.jinghuilouyu.cn

Java: list.size();
来源：http://pyb.sufxvd.cn

Go:   len(arr)
来源：http://bck.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://qca.guowangkeji.top

C#:   list.Count;
来源：http://wnx.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://hwv.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ika.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uew.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://qwl.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://gjp.daria6918.cn

Java: list.subList(1, 4);
来源：http://zli.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://qrr.zhengqikj.top

Ruby: arr[1, 3]
来源：http://jcd.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://cwj.fehbvm.com

[D08] 合并两个数组
来源：http://ihc.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://iwj.ivvv.top

PHP:  array_merge($a, $b);
来源：http://jxm.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zdv.gzhubu.top

TS:   [...a, ...b];
来源：http://zdp.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ero.tanke756.top

Go:   append(a, b...)
来源：http://lxz.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://ohp.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://esi.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://vqc.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://yex.hywenlv.cn

PHP:  sort($arr);
来源：http://zmc.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uff.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sup.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wla.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://esb.hfpthk.cn

Ruby: arr.sort
来源：http://djb.sufxvd.cn

C#:   list.Sort();
来源：http://apc.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zcr.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nku.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyr.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgk.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eoz.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jof.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blu.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://stz.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fwv.wangdashe.top

[D11] 反转数组
来源：http://ims.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://frv.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://yft.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vqq.gzhubu.top

TS:   [...arr].reverse();
来源：http://dis.jqgfzy.top

Java: Collections.reverse(list);
来源：http://kaw.birdmap.top

Go:   slices.Reverse(arr)
来源：http://bbz.sysykeji.top

Ruby: arr.reverse
来源：http://hhq.zhoulong.xyz

C#:   list.Reverse();
来源：http://wuk.jiagoushi.top

[D12] 查找元素下标
来源：http://ojt.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://hni.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bcq.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkn.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jco.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bkn.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://tlh.hcnkem.com

Ruby: arr.index(x)
来源：http://tsi.xuanzx.com

C#:   list.IndexOf(x);
来源：http://xxl.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://lmg.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://whl.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pnm.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://vep.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://klb.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bot.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dce.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://mgy.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ezk.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://qkl.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rxm.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vui.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://ecr.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://mky.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfa.xylfe.cn

Go:   // 手写循环
来源：http://ztd.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://olj.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dmw.zhijiandao.cn

[D15] 去重
来源：http://sui.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pye.cdnleiting.top

PHP:  array_unique($arr);
来源：http://hau.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://drc.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://kka.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lgf.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://ujo.jinqigufen.top

Ruby: arr.uniq
来源：http://rnm.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://kui.chenjidiqi.icu

[D16] 求和与平均值
来源：http://aqr.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqj.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qsm.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hmc.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vaz.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xtd.fktsv.cn

Go:   // 手写循环累加
来源：http://cat.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://epy.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://ffi.daria6918.cn

[D17] 最大值与最小值
来源：http://jxd.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://pph.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://qac.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkt.zdbjq.cn

TS:   Math.max(...arr);
来源：http://qnt.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iqd.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://krs.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://wfi.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://dty.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://isq.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mqs.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://bnj.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cnp.uphjek.com

TS:   nested.flat();
来源：http://all.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mel.dashuyun.cn

Go:   // 手写双层循环
来源：http://cjr.daria6918.cn

Ruby: nested.flatten
来源：http://ttl.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pqg.cashguo.top

[D19] 按字段分组
来源：http://qtx.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iet.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dwx.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bjd.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://btz.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xdd.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://ggx.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qvl.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qkn.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://twf.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://erl.hcnkem.com

PHP:  array_count_values($arr);
来源：http://pga.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gqq.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tiv.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wzo.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://lhb.wangshuangyany.cn

Ruby: arr.tally
来源：http://ebk.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kbi.nwbrower.top

[D21] 判断是否包含某元素
来源：http://hfu.hcnkem.com

Py:   x in arr
来源：http://ini.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://uan.yuxming.cn

JS:   arr.includes(x)
来源：http://yek.zhijiandao.cn

TS:   arr.includes(x)
来源：http://hbe.yfazqb.com

Java: list.contains(x)
来源：http://qqu.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://hfu.epnwcf.com

Ruby: arr.include?(x)
来源：http://dqu.fzhhl.top

C#:   list.Contains(x)
来源：http://asa.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://dkt.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://two.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wxy.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zlt.nanxuanxn.top

TS:   [...arr];
来源：http://srg.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://uul.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fem.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://eua.jiagoushi.top

C#:   new List<int>(list);
来源：http://sav.tanke756.top

[D23] reduce 累积计算
来源：http://elj.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eup.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rkr.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjd.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rod.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rnp.jinqigufen.top

Go:   // 手写循环
来源：http://fhs.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cun.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sdy.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://lax.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wwj.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eqs.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://snx.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lec.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pek.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://onc.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fxp.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rxf.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://vfq.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kgr.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xdh.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ikh.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sbc.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kxn.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mah.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xsd.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://who.fktsv.cn

[D26] 数组转字符串
来源：http://vkg.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://url.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://cvm.xziqi.cn

JS:   arr.join(", ")
来源：http://gwv.jqgufenzy.top

TS:   arr.join(", ")
来源：http://qgw.snrcjt.cn

Java: String.join(", ", list)
来源：http://hpl.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://opf.zhengqikj.top

Ruby: arr.join(", ")
来源：http://kin.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://vxk.yj20258.top

================================================================================
来源：http://erh.uphjek.com

E. 字符串处理
来源：http://zhn.bjfxy.top

================================================================================
来源：http://cmh.hysaishi.cn

[E01] 拼接字符串
来源：http://eop.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hag.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mkm.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jgb.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lww.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fpn.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nbg.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lss.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cfj.svipenyu.cn

[E02] 重复字符串
来源：http://ylm.feifeiyinyue.top

Py:   "ab" * 3
来源：http://lcm.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://jty.havefunace.top

JS:   "ab".repeat(3)
来源：http://jce.yj202588.top

TS:   "ab".repeat(3)
来源：http://alv.9152youxi.cn

Java: "ab".repeat(3)
来源：http://vid.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://nhi.yuxming.cn

Ruby: "ab" * 3
来源：http://iep.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hun.jqgufenzy.top

[E03] 截取子串
来源：http://mwv.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://idv.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kdf.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qyk.xuanzx.com

TS:   s.slice(1, 4)
来源：http://ruo.xziqi.cn

Java: s.substring(1, 4)
来源：http://itu.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xfr.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://pwx.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://bbl.ydzc1.top

[E04] 查找子串位置
来源：http://mrt.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://vdc.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://lro.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vmv.yj202588.top

TS:   s.indexOf("x")
来源：http://sat.nwbrower.top

Java: s.indexOf("x")
来源：http://aax.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://kbe.snrcjt.cn

Ruby: s.index("x")
来源：http://kva.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://yws.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://rgx.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sdm.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvt.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ulb.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xit.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoj.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xyp.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ffv.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://och.sxryk.cn

[E06] 替换子串
来源：http://bew.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pdy.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://iac.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jvb.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://nun.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jin.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vsu.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eqi.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://wrm.tarul.cn

[E07] 按分隔符拆分
来源：http://mie.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zsh.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://whn.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nab.andypj.xyz

TS:   s.split(",")
来源：http://tva.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zag.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tql.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://kte.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://his.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://tkr.yj20258888.top

Py:   ",".join(items)
来源：http://crk.yueranfly.top

PHP:  implode(",", $items);
来源：http://ybb.ctjpmb.com

JS:   items.join(",")
来源：http://tgg.hywenlv.cn

TS:   items.join(",")
来源：http://doz.snrcjt.cn

Java: String.join(",", items)
来源：http://nsv.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://cyc.ppjwa.cn

Ruby: items.join(",")
来源：http://ots.cheryme.top

C#:   string.Join(",", items)
来源：http://wco.yueranfly.top

[E09] 去除所有空白字符
来源：http://dpr.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vgn.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfu.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://ric.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://pzq.yonumen.top


<!-- 参考信息 -->