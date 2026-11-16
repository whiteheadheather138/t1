代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gdy.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ekn.andypj.xyz

[D05] 访问与修改元素
来源：http://gjm.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tfo.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jpw.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wns.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://cxh.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://kgl.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://iss.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fdj.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zzn.zhiwuduotai.top

[D06] 数组长度
来源：http://orj.tian-w.cn

Py:   len(arr)
来源：http://ffi.wangdashe.top

PHP:  count($arr);
来源：http://dzv.cucudq.cn

JS:   arr.length
来源：http://vdf.haohaochexian.top

TS:   arr.length
来源：http://bvo.chenzaomai.com

Java: list.size();
来源：http://nzp.yueranfly.top

Go:   len(arr)
来源：http://zze.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://rnx.yonumen.top

C#:   list.Count;
来源：http://pmt.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://vkr.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xhh.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ise.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://ehj.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://bjx.hcnkem.com

Java: list.subList(1, 4);
来源：http://jkn.havefunace.top

Go:   arr[1:4]
来源：http://idz.shuidangran.top

Ruby: arr[1, 3]
来源：http://kwr.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://kxp.chenzaomai.com

[D08] 合并两个数组
来源：http://ukr.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://urr.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://kgk.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://owy.fzhhl.top

TS:   [...a, ...b];
来源：http://pyo.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smw.aibaodan.cn

Go:   append(a, b...)
来源：http://ccd.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://soz.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://bda.hcnkem.com

[D09] 排序（升序）
来源：http://guc.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ice.cdnleiting.top

PHP:  sort($arr);
来源：http://kzn.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xte.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lxk.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hkh.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kwx.jinqigufen.top

Ruby: arr.sort
来源：http://rji.zdbjq.cn

C#:   list.Sort();
来源：http://tju.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pky.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nbk.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dch.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kmw.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://osw.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vav.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qea.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fat.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://joj.yj20258.top

[D11] 反转数组
来源：http://lcg.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://bvw.jianghu66.top

PHP:  array_reverse($arr);
来源：http://nwx.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kky.yuxming.cn

TS:   [...arr].reverse();
来源：http://enw.meibo888.top

Java: Collections.reverse(list);
来源：http://lbo.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://zme.yuxming.cn

Ruby: arr.reverse
来源：http://qie.daria6918.cn

C#:   list.Reverse();
来源：http://alw.smart0.xyz

[D12] 查找元素下标
来源：http://bez.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://ceo.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sma.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vei.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdn.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fdx.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://zlp.zhengqikj.top

Ruby: arr.index(x)
来源：http://jzz.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://qxi.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://eld.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ohm.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wnv.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://nau.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://ykn.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oho.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cxz.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://fxy.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://elj.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://iov.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://siz.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tfk.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://qyu.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://yfz.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://acp.zhongyouzk.top

Go:   // 手写循环
来源：http://yfi.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rsr.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zly.meibo888.top

[D15] 去重
来源：http://svs.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gki.hesvh.cn

PHP:  array_unique($arr);
来源：http://vyr.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://qeo.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://edu.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://keu.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://lya.ivvv.top

Ruby: arr.uniq
来源：http://wen.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://egb.yvedp.cn

[D16] 求和与平均值
来源：http://vbt.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cgn.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wxj.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iod.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqb.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yzd.nanxuanxn.top

Go:   // 手写循环累加
来源：http://dew.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://irk.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://czw.guannengcc.top

[D17] 最大值与最小值
来源：http://ljn.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://xum.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://deu.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bbl.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://qut.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rew.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qix.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://etq.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://bwo.cheryme.top

[D18] 扁平化嵌套数组
来源：http://ybq.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://elu.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://hge.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://joi.fzhhl.top

TS:   nested.flat();
来源：http://dvw.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wep.zhengqikj.top

Go:   // 手写双层循环
来源：http://xlu.52xcode.cn

Ruby: nested.flatten
来源：http://syt.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vip.xuetiantiany.cn

[D19] 按字段分组
来源：http://amb.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jji.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mws.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fwu.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sbn.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sox.sweek.top

Go:   // 手写 map[string][]T
来源：http://whi.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://soz.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izo.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://owc.xinyue.icu

Py:   Counter(arr)
来源：http://fru.yvedp.cn

PHP:  array_count_values($arr);
来源：http://acf.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://are.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nfi.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://izt.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://ziq.xuanzx.com

Ruby: arr.tally
来源：http://kia.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qhn.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://adv.wangshuangyany.cn

Py:   x in arr
来源：http://vqp.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://egi.zhijiandao.cn

JS:   arr.includes(x)
来源：http://fhc.fehbvm.com

TS:   arr.includes(x)
来源：http://maw.tian-w.cn

Java: list.contains(x)
来源：http://fkf.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://jlz.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://iej.gogol.net.cn

C#:   list.Contains(x)
来源：http://auz.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://emo.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://puq.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pex.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://knu.fktsv.cn

TS:   [...arr];
来源：http://mee.smart0.xyz

Java: new ArrayList<>(list);
来源：http://hqo.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://idd.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://jmp.sweek.top

C#:   new List<int>(list);
来源：http://hyi.sufxvd.cn

[D23] reduce 累积计算
来源：http://rdq.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://unu.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qxe.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skn.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thh.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgp.zhongyouzk.top

Go:   // 手写循环
来源：http://dds.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wwj.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ddj.sweek.top

[D24] 字典 / Map 基本操作
来源：http://xtl.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ayz.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eat.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tgo.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://itq.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://trr.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ena.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nat.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nyl.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://zct.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rzy.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://had.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxf.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbx.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ysl.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zxi.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rlw.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bal.sjlbkw.cn

[D26] 数组转字符串
来源：http://euw.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://rcb.uphjek.com

PHP:  implode(", ", $arr);
来源：http://xoy.fengsongda.top

JS:   arr.join(", ")
来源：http://qmt.fktsv.cn

TS:   arr.join(", ")
来源：http://rrc.xinyue.icu

Java: String.join(", ", list)
来源：http://oth.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://eiw.yuanzhike.top

Ruby: arr.join(", ")
来源：http://cqb.sysykeji.top

C#:   string.Join(", ", list)
来源：http://cha.fengsongda.top

================================================================================
来源：http://wpd.vqdsnc.cn

E. 字符串处理
来源：http://rgj.jinqigfzy.top

================================================================================
来源：http://xjq.zhengqikj.top

[E01] 拼接字符串
来源：http://hon.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://efe.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rzv.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jrp.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfu.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ejx.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iho.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fhe.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://krk.52xcode.cn

[E02] 重复字符串
来源：http://qdt.fengsongda.top

Py:   "ab" * 3
来源：http://awt.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://rzw.xylfe.cn

JS:   "ab".repeat(3)
来源：http://asp.yuxming.cn

TS:   "ab".repeat(3)
来源：http://uvr.yonumen.top

Java: "ab".repeat(3)
来源：http://vxg.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://aaw.jiagoushi.top

Ruby: "ab" * 3
来源：http://ixb.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xjs.0kj1m.cn

[E03] 截取子串
来源：http://via.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zqx.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mrl.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jtl.52xcode.cn

TS:   s.slice(1, 4)
来源：http://ljj.bjfxy.top

Java: s.substring(1, 4)
来源：http://ahg.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fwu.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zgl.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://gem.zhengqikj.top

[E04] 查找子串位置
来源：http://zxi.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://noz.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://eip.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nba.sufxvd.cn

TS:   s.indexOf("x")
来源：http://ssk.shuidangran.top

Java: s.indexOf("x")
来源：http://uua.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://gpo.pycfn.com

Ruby: s.index("x")
来源：http://nwx.yj20258.top

C#:   s.IndexOf("x")
来源：http://kld.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqi.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wzw.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://spb.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxp.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zym.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wae.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jjt.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://png.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwj.yangfankeji.com

[E06] 替换子串
来源：http://msr.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qqu.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://eap.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jtv.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://blg.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oic.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tev.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vem.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://uyj.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://hug.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mue.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqr.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxp.nwbrower.top

TS:   s.split(",")
来源：http://ldd.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://wnh.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dnv.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://qbr.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lsb.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://ufp.hfpthk.cn

Py:   ",".join(items)
来源：http://axm.cqqwz.cn

PHP:  implode(",", $items);
来源：http://dwi.jyoumei.cn

JS:   items.join(",")
来源：http://arc.tanke756.top

TS:   items.join(",")
来源：http://zwz.aibaodan.cn

Java: String.join(",", items)
来源：http://yvy.meibo888.top

Go:   strings.Join(items, ",")
来源：http://yzy.xinyue.icu

Ruby: items.join(",")
来源：http://krk.dashuyun.cn

C#:   string.Join(",", items)
来源：http://zsm.yonumen.top

[E09] 去除所有空白字符
来源：http://lcr.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tga.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qov.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://ive.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://qlm.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://kie.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kni.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://yxe.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bfz.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://vsr.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bpg.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vto.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://pdx.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://wzn.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://paj.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dkb.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rpu.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gra.zdqjudy.top

[E11] 反转字符串
来源：http://lma.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://lcp.tanke756.top

PHP:  strrev($s);
来源：http://nek.tanke756.top

JS:   [...s].reverse().join("")
来源：http://ckq.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://izh.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://agt.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lcz.zhongyouzk.top


<!-- 参考信息 -->