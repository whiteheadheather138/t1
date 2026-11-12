代发 wailian999

[D03] 在指定位置插入元素
来源：http://nzb.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://wdh.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lhk.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wit.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://lvu.yuanzhike.top

Java: list.add(0, 0);
来源：http://dnf.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lxq.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oip.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://stx.ywan-chungtsiang.top

[D04] 删除元素
来源：http://dqr.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qos.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ltu.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cfy.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://cfa.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yer.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://raz.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://scm.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lcb.jiagoushi.top

[D05] 访问与修改元素
来源：http://gnb.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cmj.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hsp.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wyv.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://clz.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://dmp.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://zgx.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hhs.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ajx.yuxming.cn

[D06] 数组长度
来源：http://alo.pengpengdd.cyou

Py:   len(arr)
来源：http://njb.jlsjyb.cn

PHP:  count($arr);
来源：http://vfy.birdmap.top

JS:   arr.length
来源：http://fbt.gotoacloud.top

TS:   arr.length
来源：http://vsz.tian-w.cn

Java: list.size();
来源：http://rfc.andypj.xyz

Go:   len(arr)
来源：http://ven.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://xjb.chenlongwang.top

C#:   list.Count;
来源：http://rzw.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://yeo.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzn.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://lfe.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://vcy.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://iir.yuxming.cn

Java: list.subList(1, 4);
来源：http://jql.ivvv.top

Go:   arr[1:4]
来源：http://uaq.epnwcf.com

Ruby: arr[1, 3]
来源：http://pxt.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://qqt.havefunace.top

[D08] 合并两个数组
来源：http://ibx.jlsjyb.cn

Py:   a + b;  a.extend(b)
来源：http://ycq.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://rvq.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://anv.jinqigufen.top

TS:   [...a, ...b];
来源：http://eli.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xkq.dianchejie.cn

Go:   append(a, b...)
来源：http://vdr.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://wxc.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://fjs.vehdjk.com

[D09] 排序（升序）
来源：http://ypl.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://taj.hnqzz.top

PHP:  sort($arr);
来源：http://gyn.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kmm.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ekg.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://peb.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://obv.dashuyun.cn

Ruby: arr.sort
来源：http://pbf.chenjidiqi.icu

C#:   list.Sort();
来源：http://qoc.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jtp.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kao.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfh.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cjy.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ody.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qeo.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bgh.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yca.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yty.hcnkem.com

[D11] 反转数组
来源：http://cwf.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://bro.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://zlj.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://afh.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://guv.hfpthk.cn

Java: Collections.reverse(list);
来源：http://jou.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://twy.aizwys.cn

Ruby: arr.reverse
来源：http://gkf.vehdjk.com

C#:   list.Reverse();
来源：http://zer.kuanghao11.cn

[D12] 查找元素下标
来源：http://sjx.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://zrp.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ojs.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfo.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tyc.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xwz.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://irl.yj20258888.top

Ruby: arr.index(x)
来源：http://wtz.cucudq.cn

C#:   list.IndexOf(x);
来源：http://ufa.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://rvl.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mdt.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eeo.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://cnn.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://tzj.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jdz.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://khf.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gbq.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jxl.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://bqg.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://huz.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbb.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://hve.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://kha.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ikc.xziqi.cn

Go:   // 手写循环
来源：http://fhk.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yju.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://hdo.dianchejie.cn

[D15] 去重
来源：http://ane.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lns.daria6918.cn

PHP:  array_unique($arr);
来源：http://spd.yfazqb.com

JS:   [...new Set(arr)]
来源：http://arz.gzhubu.top

TS:   [...new Set(arr)]
来源：http://hkm.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxp.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://dpj.chenjidiqi.icu

Ruby: arr.uniq
来源：http://ytu.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://nem.pycfn.com

[D16] 求和与平均值
来源：http://omy.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ybl.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pbo.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ysi.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xxq.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mqc.zycfv.cn

Go:   // 手写循环累加
来源：http://srr.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjt.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://ngb.fengsongda.top

[D17] 最大值与最小值
来源：http://lai.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://aew.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://rwa.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qcx.haohaochexian.top

TS:   Math.max(...arr);
来源：http://jav.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wxo.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://slw.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://ivx.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://mqx.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://qcp.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iyt.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://keo.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bah.dashuyun.cn

TS:   nested.flat();
来源：http://sib.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cel.tarul.cn

Go:   // 手写双层循环
来源：http://mgf.smart0.xyz

Ruby: nested.flatten
来源：http://rjb.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://jyc.quarkkingdee.top

[D19] 按字段分组
来源：http://hmw.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oxr.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://isw.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ufh.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fnu.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rji.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://qkh.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://aui.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jlb.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://tvs.sxryk.cn

Py:   Counter(arr)
来源：http://cpo.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://six.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fod.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpm.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kch.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://wdi.ybcxt.top

Ruby: arr.tally
来源：http://opt.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wsp.c1oappe.top

[D21] 判断是否包含某元素
来源：http://gel.nwbrower.top

Py:   x in arr
来源：http://mdf.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://zss.hnqzz.top

JS:   arr.includes(x)
来源：http://qoo.epnwcf.com

TS:   arr.includes(x)
来源：http://ogc.fktsv.cn

Java: list.contains(x)
来源：http://hfq.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://txl.xziqi.cn

Ruby: arr.include?(x)
来源：http://amh.hywenlv.cn

C#:   list.Contains(x)
来源：http://dzn.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://wua.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pgt.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zvq.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cvg.yj20258.top

TS:   [...arr];
来源：http://fze.xylfe.cn

Java: new ArrayList<>(list);
来源：http://jcy.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://oqd.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://hxd.zhijiandao.cn

C#:   new List<int>(list);
来源：http://wyu.daria6918.cn

[D23] reduce 累积计算
来源：http://tlp.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iaq.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://igd.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ymh.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mod.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yzn.daria6918.cn

Go:   // 手写循环
来源：http://zhj.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ajj.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wxc.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://eni.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aqe.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://juv.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qra.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zxl.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lqi.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fyq.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oht.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xdb.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://iim.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hhq.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://opa.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://abx.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://diz.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uga.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mmg.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://izh.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tid.yanxiufei.cn

[D26] 数组转字符串
来源：http://dmq.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://ote.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://pfw.zycfv.cn

JS:   arr.join(", ")
来源：http://sbt.cdnleiting.top

TS:   arr.join(", ")
来源：http://ctg.chenzaomai.com

Java: String.join(", ", list)
来源：http://hgk.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://aaw.yonumen.top

Ruby: arr.join(", ")
来源：http://pqq.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://wge.shuidangran.top

================================================================================
来源：http://cia.yfazqb.com

E. 字符串处理
来源：http://cjk.meibo888.top

================================================================================
来源：http://mnv.sjlbkw.cn

[E01] 拼接字符串
来源：http://hjl.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://daf.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rlo.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cme.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grx.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gry.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jxd.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://elz.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blf.yongpay.top

[E02] 重复字符串
来源：http://zrn.yueranfly.top

Py:   "ab" * 3
来源：http://cjc.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://qqr.vehdjk.com

JS:   "ab".repeat(3)
来源：http://fso.hammf.cn

TS:   "ab".repeat(3)
来源：http://eta.sysykeji.top

Java: "ab".repeat(3)
来源：http://gqc.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://azx.ydzc1.top

Ruby: "ab" * 3
来源：http://xsn.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mnp.zhiwuduotai.top

[E03] 截取子串
来源：http://vkf.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xrr.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hjb.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://znn.ybcxt.top

TS:   s.slice(1, 4)
来源：http://mom.daxiang520.top

Java: s.substring(1, 4)
来源：http://twx.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ics.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://bir.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://fot.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://zwy.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://oxp.vehdjk.com

PHP:  strpos($s, "x");
来源：http://nzj.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://guu.havefunace.top

TS:   s.indexOf("x")
来源：http://gba.smart0.xyz

Java: s.indexOf("x")
来源：http://dqj.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://nlv.yongpay.top

Ruby: s.index("x")
来源：http://uqa.sxryk.cn

C#:   s.IndexOf("x")
来源：http://vcg.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kea.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eay.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oxw.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xww.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://emp.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxe.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dtn.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xyu.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sum.fehbvm.com

[E06] 替换子串
来源：http://ode.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tbw.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://gtz.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sue.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://nsg.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pff.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://unt.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jhq.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://yck.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://gut.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ziu.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aya.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xjm.yanxiufei.cn

TS:   s.split(",")
来源：http://mud.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uwz.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qww.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://pdp.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dnl.c1oappe.top

[E08] 数组按分隔符合并
来源：http://xof.quarkkingdee.top

Py:   ",".join(items)
来源：http://sdy.c1oappe.top

PHP:  implode(",", $items);
来源：http://inu.ctjpmb.com

JS:   items.join(",")
来源：http://mht.pycfn.com

TS:   items.join(",")
来源：http://ffp.gogol.net.cn

Java: String.join(",", items)
来源：http://gmo.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://kel.ybcxt.top

Ruby: items.join(",")
来源：http://pcx.ppjwa.cn

C#:   string.Join(",", items)
来源：http://cjw.c1oappe.top

[E09] 去除所有空白字符
来源：http://wzg.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oex.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xnh.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://kqu.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://ydk.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://vml.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://act.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://big.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cnb.hywenlv.cn


<!-- 参考信息 -->