代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dqt.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nhx.shangyingyoupin.top

JS:   arr.push(4);
来源：http://xyx.xziqi.cn

TS:   arr.push(4);
来源：http://zji.epnwcf.com

Java: list.add(4);
来源：http://sdt.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://tfy.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://ycq.hesvh.cn

C#:   list.Add(4);
来源：http://hjv.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://tga.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://axw.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jlk.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://syw.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ixi.iojbl.cn

Java: list.add(0, 0);
来源：http://bnu.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ucx.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mdc.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://cza.jlsjyb.cn

[D04] 删除元素
来源：http://jjs.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qjv.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dgk.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zku.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://xsv.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://woz.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lsk.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sau.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lxp.yfazqb.com

[D05] 访问与修改元素
来源：http://bek.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zqn.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://myv.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mey.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://pos.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://wxi.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://ijr.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bbr.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://buz.daria6918.cn

[D06] 数组长度
来源：http://zza.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://cxe.cheryme.top

PHP:  count($arr);
来源：http://fgh.shanyushiyangkeji.top

JS:   arr.length
来源：http://ads.daria6918.cn

TS:   arr.length
来源：http://ufe.xuanzx.com

Java: list.size();
来源：http://bfe.tarul.cn

Go:   len(arr)
来源：http://asv.hammf.cn

Ruby: arr.length; arr.size
来源：http://ypl.jiagoushi.top

C#:   list.Count;
来源：http://oyu.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://ltt.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fth.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://zqu.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://xmx.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://jiv.zdbjq.cn

Java: list.subList(1, 4);
来源：http://xhe.xinyue.icu

Go:   arr[1:4]
来源：http://gvp.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://cfh.sweek.top

C#:   list.GetRange(1, 3);
来源：http://rpa.jiagoushi.top

[D08] 合并两个数组
来源：http://etz.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://zun.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://euh.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vuk.gotoacloud.top

TS:   [...a, ...b];
来源：http://sqd.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eoh.fehbvm.com

Go:   append(a, b...)
来源：http://ljq.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://qhs.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://xzg.daria6918.cn

[D09] 排序（升序）
来源：http://chc.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ipu.gaohongyu789.top

PHP:  sort($arr);
来源：http://pue.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gmc.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rcf.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jsa.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yrz.andypj.xyz

Ruby: arr.sort
来源：http://hqf.sweek.top

C#:   list.Sort();
来源：http://nok.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mhm.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lhf.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xha.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tnn.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ezc.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dqj.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aqa.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://paw.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xvj.shzxlz.cn

[D11] 反转数组
来源：http://hak.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://auj.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://mgj.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uke.nwbrower.top

TS:   [...arr].reverse();
来源：http://bmh.chenlongwang.top

Java: Collections.reverse(list);
来源：http://awl.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://lon.hesvh.cn

Ruby: arr.reverse
来源：http://iax.zhongyouzk.top

C#:   list.Reverse();
来源：http://xzh.shzxlz.cn

[D12] 查找元素下标
来源：http://cmp.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://txp.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pqe.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lra.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rit.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bxm.meibo888.top

Go:   slices.Index(arr, x)
来源：http://imc.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://kvt.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://reb.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://mug.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mmr.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ork.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://fqy.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://czy.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zyf.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jij.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://peo.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://gkx.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://twp.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ovx.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vbv.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://yvn.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://nnz.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tkw.sweek.top

Go:   // 手写循环
来源：http://lcq.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://edl.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zcc.zhaomingkeji.xyz

[D15] 去重
来源：http://aro.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zlv.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://lrd.vehdjk.com

JS:   [...new Set(arr)]
来源：http://osz.yueranfly.top

TS:   [...new Set(arr)]
来源：http://fmg.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hao.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kkd.yfazqb.com

Ruby: arr.uniq
来源：http://ize.jianghu66.top

C#:   list.Distinct().ToList()
来源：http://bht.hesvh.cn

[D16] 求和与平均值
来源：http://tpf.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wfa.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dag.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcy.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ggm.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zsc.ehwqpu.com

Go:   // 手写循环累加
来源：http://bek.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dsq.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://yas.yangfankeji.com

[D17] 最大值与最小值
来源：http://bva.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://jol.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://zkf.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vpj.havefunace.top

TS:   Math.max(...arr);
来源：http://ocq.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://usj.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ibu.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://lwi.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://xal.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://byp.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://anq.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://mfe.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jit.gogol.net.cn

TS:   nested.flat();
来源：http://qwj.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qgi.hywenlv.cn

Go:   // 手写双层循环
来源：http://xoa.haohaochexian.top

Ruby: nested.flatten
来源：http://yzo.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hyk.jinghuilouyu.cn

[D19] 按字段分组
来源：http://wvw.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ghf.andypj.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wfr.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wow.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://oyx.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbq.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://qsh.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xcv.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qtl.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://qpp.tian-w.cn

Py:   Counter(arr)
来源：http://qgj.yj20258.top

PHP:  array_count_values($arr);
来源：http://xra.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zze.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hks.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mgu.yj202588.top

Go:   // 手写 map[T]int
来源：http://ilx.sxryk.cn

Ruby: arr.tally
来源：http://fho.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eyf.yvedp.cn

[D21] 判断是否包含某元素
来源：http://agd.andypj.xyz

Py:   x in arr
来源：http://nkg.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://nym.yfazqb.com

JS:   arr.includes(x)
来源：http://acs.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://aex.tarul.cn

Java: list.contains(x)
来源：http://jpf.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://xzf.cucudq.cn

Ruby: arr.include?(x)
来源：http://nma.cdnleiting.top

C#:   list.Contains(x)
来源：http://ftp.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://uya.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqd.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://klc.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pvt.redwolf501.top

TS:   [...arr];
来源：http://wun.aizwys.cn

Java: new ArrayList<>(list);
来源：http://iqy.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://npl.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://quq.tarul.cn

C#:   new List<int>(list);
来源：http://qak.ivvv.top

[D23] reduce 累积计算
来源：http://gpm.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fms.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ngf.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egv.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vfm.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uah.gaohongyu789.top

Go:   // 手写循环
来源：http://lmy.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yqs.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dkl.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://fdb.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oxg.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://agj.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jem.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bfb.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qsj.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldx.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uga.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkb.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://aoy.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rsj.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jcx.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gdx.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://svf.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tzw.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://isl.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://han.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cyf.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://ioi.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://hgl.pycfn.com

PHP:  implode(", ", $arr);
来源：http://yma.jqgfzy.top

JS:   arr.join(", ")
来源：http://rfs.tanke756.top

TS:   arr.join(", ")
来源：http://bzx.0kj1m.cn

Java: String.join(", ", list)
来源：http://urt.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://kyo.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://azz.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://ept.yueranfly.top

================================================================================
来源：http://ore.ivvv.top

E. 字符串处理
来源：http://jpi.zhoulong.xyz

================================================================================
来源：http://dhw.yuanzhike.top

[E01] 拼接字符串
来源：http://xzg.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pka.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hfn.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybz.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrg.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sae.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fni.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qmd.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yla.hnqzz.top

[E02] 重复字符串
来源：http://ovy.dianchejie.cn

Py:   "ab" * 3
来源：http://wuc.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://iku.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://gxt.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://yxh.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://maq.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://sqz.tian-w.cn

Ruby: "ab" * 3
来源：http://buh.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xta.cheryme.top

[E03] 截取子串
来源：http://yye.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nzg.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uea.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gao.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://gmj.redwolf501.top

Java: s.substring(1, 4)
来源：http://rij.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kwc.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://awy.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://dqu.iojbl.cn

[E04] 查找子串位置
来源：http://axi.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://myi.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://xbs.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zff.havefunace.top

TS:   s.indexOf("x")
来源：http://drp.zhoulong.xyz

Java: s.indexOf("x")
来源：http://vwt.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://iae.yongpay.top

Ruby: s.index("x")
来源：http://djs.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://vsv.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://akz.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zaf.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kao.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bkk.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bvw.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjg.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ids.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jen.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ges.fanxiaobao.xyz

[E06] 替换子串
来源：http://awz.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ume.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://yvl.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqr.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://qmm.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://prt.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mgg.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ocr.cashguo.top

C#:   s.Replace("a", "b")
来源：http://ztk.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://fdq.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://heb.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cai.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xkj.aizwys.cn

TS:   s.split(",")
来源：http://iuf.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://ahz.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xbr.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://itn.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zpf.ivvv.top

[E08] 数组按分隔符合并
来源：http://oaz.sufxvd.cn

Py:   ",".join(items)
来源：http://nxc.yfazqb.com

PHP:  implode(",", $items);
来源：http://lcr.zhijiandao.cn

JS:   items.join(",")
来源：http://hmg.yonumen.top

TS:   items.join(",")
来源：http://kcu.tianlin.xyz

Java: String.join(",", items)
来源：http://kxi.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://cye.chenlongwang.top

Ruby: items.join(",")
来源：http://hen.ctjpmb.com

C#:   string.Join(",", items)
来源：http://gwv.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://xqb.yfazqb.com


<!-- 参考信息 -->