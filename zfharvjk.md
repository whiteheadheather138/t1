代发 wailian999

Py:   len(arr)
来源：http://wcv.jianghu66.top

PHP:  count($arr);
来源：http://kab.chenlongwang.top

JS:   arr.length
来源：http://zhu.zhengqikj.top

TS:   arr.length
来源：http://zac.hnxiangtu.top

Java: list.size();
来源：http://dhz.cheryme.top

Go:   len(arr)
来源：http://ggn.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://wuq.uphjek.com

C#:   list.Count;
来源：http://rnd.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://lml.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://shq.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qzp.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://oiz.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://zja.zhixingplan.top

Java: list.subList(1, 4);
来源：http://twp.nanxuanxn.top

Go:   arr[1:4]
来源：http://wrh.xuanzx.com

Ruby: arr[1, 3]
来源：http://wqw.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://mda.guowangkeji.top

[D08] 合并两个数组
来源：http://rvo.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://ycq.uphjek.com

PHP:  array_merge($a, $b);
来源：http://loy.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ihh.jinqigufen.top

TS:   [...a, ...b];
来源：http://dpo.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oso.chenjidiqi.icu

Go:   append(a, b...)
来源：http://kzb.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://idh.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://frd.yueranfly.top

[D09] 排序（升序）
来源：http://fcc.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://aau.sysykeji.top

PHP:  sort($arr);
来源：http://whj.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qdl.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zxb.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vmj.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://txg.zhijiandao.cn

Ruby: arr.sort
来源：http://ywn.cqqwz.cn

C#:   list.Sort();
来源：http://adk.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kee.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffm.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yij.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcc.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nsc.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zze.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dtz.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://djv.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fju.yangfankeji.com

[D11] 反转数组
来源：http://jvo.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://lkb.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://eph.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qhd.ctjpmb.com

TS:   [...arr].reverse();
来源：http://dhe.ydzc1.top

Java: Collections.reverse(list);
来源：http://sot.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://hcl.cdnleiting.top

Ruby: arr.reverse
来源：http://rss.sjlbkw.cn

C#:   list.Reverse();
来源：http://mfh.hnqzz.top

[D12] 查找元素下标
来源：http://myh.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://kfx.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sdb.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zld.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tjt.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tkm.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://lcb.iojbl.cn

Ruby: arr.index(x)
来源：http://yta.bbcook.cn

C#:   list.IndexOf(x);
来源：http://jqo.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://lpi.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ywf.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pmj.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://wjm.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://wqe.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zlu.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fks.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://qog.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nep.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://gfj.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aky.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kxl.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://xno.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://eec.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rrc.jqgufenzy.top

Go:   // 手写循环
来源：http://pbr.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://vsw.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ifk.ivvv.top

[D15] 去重
来源：http://zqc.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xvd.yonumen.top

PHP:  array_unique($arr);
来源：http://toz.jianghu66.top

JS:   [...new Set(arr)]
来源：http://trk.sweek.top

TS:   [...new Set(arr)]
来源：http://yxn.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tbb.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qyz.daria6918.cn

Ruby: arr.uniq
来源：http://gkq.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://hrx.quarkkingdee.top

[D16] 求和与平均值
来源：http://wae.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dew.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://brf.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://irq.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppp.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ncl.dianchejie.cn

Go:   // 手写循环累加
来源：http://pxu.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dhx.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://qyj.nanxuanxn.top

[D17] 最大值与最小值
来源：http://vhp.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://wfw.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://aao.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://euo.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://pdc.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cpi.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pku.cheryme.top

Ruby: arr.max;  arr.min
来源：http://sjd.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://upd.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://knn.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dno.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://elj.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fsg.aibaodan.cn

TS:   nested.flat();
来源：http://rjc.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zuh.vehdjk.com

Go:   // 手写双层循环
来源：http://hqc.aibaodan.cn

Ruby: nested.flatten
来源：http://gbs.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yki.zhijiandao.cn

[D19] 按字段分组
来源：http://tog.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xeg.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kuc.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nht.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vqn.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rii.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://usk.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://wyy.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pjj.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://bxf.xuetiantiany.cn

Py:   Counter(arr)
来源：http://haz.316326.xyz

PHP:  array_count_values($arr);
来源：http://ent.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rqx.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yek.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnr.yvedp.cn

Go:   // 手写 map[T]int
来源：http://fxk.cheryme.top

Ruby: arr.tally
来源：http://oiq.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hyj.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://udf.epnwcf.com

Py:   x in arr
来源：http://noy.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://ndw.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://yuz.yj202588.top

TS:   arr.includes(x)
来源：http://fmv.xylfe.cn

Java: list.contains(x)
来源：http://edu.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://uil.meibo888.top

Ruby: arr.include?(x)
来源：http://akl.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://zrs.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://wjf.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ccq.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ubl.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bph.ehwqpu.com

TS:   [...arr];
来源：http://bcr.smart0.xyz

Java: new ArrayList<>(list);
来源：http://dtm.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://tbo.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://asb.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://qpc.ydzc1.top

[D23] reduce 累积计算
来源：http://ash.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jpi.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uny.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmo.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oxf.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ybg.tianlin.xyz

Go:   // 手写循环
来源：http://bgq.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mzf.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fni.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://hcc.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vef.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pky.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fmk.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ype.haohaochexian.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gxh.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ebl.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://goz.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qqf.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://glw.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mvi.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gki.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvn.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xfs.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eok.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nlp.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://duf.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hfl.jyoumei.cn

[D26] 数组转字符串
来源：http://vwu.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://ysi.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://khg.ydjk.org.cn

JS:   arr.join(", ")
来源：http://psu.cdnleiting.top

TS:   arr.join(", ")
来源：http://isn.fehbvm.com

Java: String.join(", ", list)
来源：http://vil.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://ytb.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://wgg.hammf.cn

C#:   string.Join(", ", list)
来源：http://nna.sufxvd.cn

================================================================================
来源：http://ear.yvedp.cn

E. 字符串处理
来源：http://wee.cheryme.top

================================================================================
来源：http://pwn.yj20258888.top

[E01] 拼接字符串
来源：http://ftw.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nbu.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dpz.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://avb.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kwv.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hxu.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nps.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rai.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ara.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://tbu.chenjidiqi.icu

Py:   "ab" * 3
来源：http://igl.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://xdk.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://wfg.meibo888.top

TS:   "ab".repeat(3)
来源：http://wre.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://piz.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://doc.hesvh.cn

Ruby: "ab" * 3
来源：http://bxd.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wzw.fehbvm.com

[E03] 截取子串
来源：http://aun.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oci.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eom.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dzx.yfazqb.com

TS:   s.slice(1, 4)
来源：http://zry.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://dky.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vbn.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://uvj.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://tzm.svipenyu.cn

[E04] 查找子串位置
来源：http://enj.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://wpk.zycfv.cn

PHP:  strpos($s, "x");
来源：http://tdr.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rwq.svipenyu.cn

TS:   s.indexOf("x")
来源：http://sow.hywenlv.cn

Java: s.indexOf("x")
来源：http://uvp.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://fwx.zhixingplan.top

Ruby: s.index("x")
来源：http://mlo.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://sts.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qri.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zyb.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rev.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jve.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hsg.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://skt.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zvp.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qne.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://exr.xuetiantiany.cn

[E06] 替换子串
来源：http://vsg.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dqv.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://kyr.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://obe.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://fkv.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sjt.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://den.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dqf.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://uek.ivvv.top

[E07] 按分隔符拆分
来源：http://znf.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lnv.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hkw.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxw.nanxuanxn.top

TS:   s.split(",")
来源：http://rdz.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ojl.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xqc.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://rpv.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tzm.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://ptg.havefunace.top

Py:   ",".join(items)
来源：http://aev.ehwqpu.com

PHP:  implode(",", $items);
来源：http://lci.hnqzz.top

JS:   items.join(",")
来源：http://hkw.chenjidiqi.icu

TS:   items.join(",")
来源：http://kns.sjlbkw.cn

Java: String.join(",", items)
来源：http://pie.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://hqb.yj20258.top

Ruby: items.join(",")
来源：http://web.yongpay.top

C#:   string.Join(",", items)
来源：http://vsy.aizwys.cn

[E09] 去除所有空白字符
来源：http://ier.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zye.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dao.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://uym.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://tar.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://iyt.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bkp.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://uek.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nja.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://lbz.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gvu.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uri.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://lbk.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://slo.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://kih.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tsx.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xvg.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pxz.cqqwz.cn

[E11] 反转字符串
来源：http://vhv.yangfankeji.com

Py:   s[::-1]
来源：http://ybi.bbcook.cn

PHP:  strrev($s);
来源：http://tpg.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://vcf.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://buj.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tza.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://meq.fzhhl.top

Ruby: s.reverse
来源：http://tee.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://orj.iojbl.cn

[E12] 统计某字符出现次数
来源：http://hot.yj20258888.top

Py:   s.count("a")
来源：http://qjv.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://vzw.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://vax.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://hpq.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvn.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://rbz.pycfn.com

Ruby: s.count("a")
来源：http://ubs.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://gjp.tanke756.top

[E13] 逐字符遍历
来源：http://dkl.shangyingyoupin.top


<!-- 参考信息 -->