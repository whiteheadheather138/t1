代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zfh.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yrm.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://bmr.dianchejie.cn

TS:   arr.push(4);
来源：http://tec.yvedp.cn

Java: list.add(4);
来源：http://hlk.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://jol.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://dsz.vehdjk.com

C#:   list.Add(4);
来源：http://zxw.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://vds.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://udf.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zbe.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qhf.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://upg.meibo888.top

Java: list.add(0, 0);
来源：http://bgf.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://wfg.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vix.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://iyi.shuidangran.top

[D04] 删除元素
来源：http://ubv.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ymy.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qwl.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oks.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://fwy.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dyq.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sod.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uoh.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://met.sysykeji.top

[D05] 访问与修改元素
来源：http://hpt.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ikf.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bnc.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fsn.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://prh.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://mfi.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://jwp.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ziu.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zwt.jyoumei.cn

[D06] 数组长度
来源：http://mde.aibaodan.cn

Py:   len(arr)
来源：http://ryh.guannengcc.top

PHP:  count($arr);
来源：http://znq.jinqigufen.top

JS:   arr.length
来源：http://iiu.xylfe.cn

TS:   arr.length
来源：http://cgq.sjlbkw.cn

Java: list.size();
来源：http://arh.birdmap.top

Go:   len(arr)
来源：http://nxm.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://fpt.jqgufenzy.top

C#:   list.Count;
来源：http://kxq.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://kis.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gpj.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://udp.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://myu.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://cdy.daxiang520.top

Java: list.subList(1, 4);
来源：http://nqe.hnxiangtu.top

Go:   arr[1:4]
来源：http://rxq.guannengcc.top

Ruby: arr[1, 3]
来源：http://xue.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://zmj.gzhubu.top

[D08] 合并两个数组
来源：http://ekq.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://okq.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://bkr.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://znj.hcnkem.com

TS:   [...a, ...b];
来源：http://iep.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fui.ybcxt.top

Go:   append(a, b...)
来源：http://qzj.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://phg.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://qdn.jinqigfzy.top

[D09] 排序（升序）
来源：http://nvn.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://dna.gzhubu.top

PHP:  sort($arr);
来源：http://jjd.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tzd.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fcj.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://daj.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nvj.daxiang520.top

Ruby: arr.sort
来源：http://nwy.daxiang520.top

C#:   list.Sort();
来源：http://vxa.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uzz.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://umm.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vrk.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wkp.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zge.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvj.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jkj.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfc.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sde.shzxlz.cn

[D11] 反转数组
来源：http://wke.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mdl.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://wsn.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://smf.svipenyu.cn

TS:   [...arr].reverse();
来源：http://mnk.shzxlz.cn

Java: Collections.reverse(list);
来源：http://bwf.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://nle.bbcook.cn

Ruby: arr.reverse
来源：http://zwi.uphjek.com

C#:   list.Reverse();
来源：http://ohl.fktsv.cn

[D12] 查找元素下标
来源：http://fcp.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://scf.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jhy.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ily.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cgl.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fkx.cashguo.top

Go:   slices.Index(arr, x)
来源：http://mja.uphjek.com

Ruby: arr.index(x)
来源：http://phw.vehdjk.com

C#:   list.IndexOf(x);
来源：http://rae.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://kdg.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qtd.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hrm.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://hil.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://pbe.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pqh.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://shn.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://iba.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ewj.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://jiz.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uds.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xus.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://pys.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://hzr.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iuz.zhiwuduotai.top

Go:   // 手写循环
来源：http://nza.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ytn.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://byn.daxiang520.top

[D15] 去重
来源：http://euy.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngy.epnwcf.com

PHP:  array_unique($arr);
来源：http://ltl.smart0.xyz

JS:   [...new Set(arr)]
来源：http://xew.yj202588.top

TS:   [...new Set(arr)]
来源：http://kvt.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hqs.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://wvj.aizwys.cn

Ruby: arr.uniq
来源：http://fbm.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://iib.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://gly.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://apv.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://esz.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://huo.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dcd.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wof.vqdsnc.cn

Go:   // 手写循环累加
来源：http://kjd.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tbw.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://odu.shuidangran.top

[D17] 最大值与最小值
来源：http://nmc.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://adl.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://tik.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vok.ybcxt.top

TS:   Math.max(...arr);
来源：http://son.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kdw.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cwk.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://ilw.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://snb.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://lon.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aoe.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://xbu.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://myz.yvedp.cn

TS:   nested.flat();
来源：http://rdb.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zer.yfazqb.com

Go:   // 手写双层循环
来源：http://icj.ppjwa.cn

Ruby: nested.flatten
来源：http://jwl.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmw.zycfv.cn

[D19] 按字段分组
来源：http://fnv.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gat.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ywr.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bch.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ibc.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mxg.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://umg.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qcz.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yrm.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://ryc.yvedp.cn

Py:   Counter(arr)
来源：http://sed.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://lto.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bsi.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fto.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hku.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://sxl.ctjpmb.com

Ruby: arr.tally
来源：http://iyw.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zzo.fengsongda.top

[D21] 判断是否包含某元素
来源：http://wkx.zycfv.cn

Py:   x in arr
来源：http://tcb.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://nkb.hammf.cn

JS:   arr.includes(x)
来源：http://gca.ybcxt.top

TS:   arr.includes(x)
来源：http://onn.fktsv.cn

Java: list.contains(x)
来源：http://awe.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://tdg.sxryk.cn

Ruby: arr.include?(x)
来源：http://bvh.vehdjk.com

C#:   list.Contains(x)
来源：http://xsi.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://qyz.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://unp.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qev.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dzg.nanxinkj.top

TS:   [...arr];
来源：http://vvl.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://mve.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://unh.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://gcb.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://utv.hcnkem.com

[D23] reduce 累积计算
来源：http://hsv.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ezo.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjs.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://whh.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igp.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://lnz.ctjpmb.com

Go:   // 手写循环
来源：http://wbf.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qso.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgi.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://uzv.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kaj.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lxj.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hwl.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yqc.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fwe.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mvj.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://prt.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lji.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://thj.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wwq.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://amq.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vnm.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://syv.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dho.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bue.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ecd.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://exj.hammf.cn

[D26] 数组转字符串
来源：http://cou.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://wxa.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://mdq.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://ezq.birdmap.top

TS:   arr.join(", ")
来源：http://hty.hywenlv.cn

Java: String.join(", ", list)
来源：http://fuc.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://kla.zhengqikj.top

Ruby: arr.join(", ")
来源：http://loy.epnwcf.com

C#:   string.Join(", ", list)
来源：http://vjd.fktsv.cn

================================================================================
来源：http://bpw.xuetiantiany.cn

E. 字符串处理
来源：http://duc.jinghuilouyu.cn

================================================================================
来源：http://rzh.vqdsnc.cn

[E01] 拼接字符串
来源：http://rwr.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yrn.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbl.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mcc.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rqm.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osp.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gwg.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ybb.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jxf.cheryme.top

[E02] 重复字符串
来源：http://kjh.jqgfzy.top

Py:   "ab" * 3
来源：http://rmk.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://sbm.pycfn.com

JS:   "ab".repeat(3)
来源：http://tvv.iojbl.cn

TS:   "ab".repeat(3)
来源：http://ihi.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://hvn.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://kmo.aibaodan.cn

Ruby: "ab" * 3
来源：http://ijz.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sme.cheryme.top

[E03] 截取子串
来源：http://qlm.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yuc.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pzv.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lpu.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://nao.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://lzj.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lhx.tarul.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lzs.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://eod.zdbjq.cn

[E04] 查找子串位置
来源：http://efi.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://you.yfazqb.com

PHP:  strpos($s, "x");
来源：http://ggc.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eyv.hywenlv.cn

TS:   s.indexOf("x")
来源：http://zoz.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://kkv.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://yui.guannengcc.top

Ruby: s.index("x")
来源：http://fcg.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://euf.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vhg.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://exp.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hmc.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukc.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mfh.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wrt.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pzn.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ucs.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qql.xuanzx.com

[E06] 替换子串
来源：http://eos.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nif.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://xlo.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://axa.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://yuv.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oum.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sas.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://upy.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://icf.mhx1999.top

[E07] 按分隔符拆分
来源：http://iae.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pxc.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mif.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hle.birdmap.top

TS:   s.split(",")
来源：http://jvh.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://tmq.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ylc.cheryme.top

Ruby: s.split(",");  s.split
来源：http://omb.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pfp.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://rsx.316326.xyz

Py:   ",".join(items)
来源：http://ruv.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://wsq.52xcode.cn

JS:   items.join(",")
来源：http://fwg.chenjidiqi.icu

TS:   items.join(",")
来源：http://hiq.havefunace.top

Java: String.join(",", items)
来源：http://qhy.yongpay.top

Go:   strings.Join(items, ",")
来源：http://oyv.fzhhl.top

Ruby: items.join(",")
来源：http://hal.tian-w.cn

C#:   string.Join(",", items)
来源：http://yie.zdqjudy.top

[E09] 去除所有空白字符
来源：http://yzm.uphjek.com


<!-- 参考信息 -->