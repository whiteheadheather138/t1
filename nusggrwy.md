代发 wailian999

[D11] 反转数组
来源：http://dpj.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://xng.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://hff.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mqg.cheryme.top

TS:   [...arr].reverse();
来源：http://lbm.zdqjudy.top

Java: Collections.reverse(list);
来源：http://jlb.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://ybx.gogol.net.cn

Ruby: arr.reverse
来源：http://ivy.tian-w.cn

C#:   list.Reverse();
来源：http://jcr.chenjidiqi.icu

[D12] 查找元素下标
来源：http://sla.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://zjz.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jac.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgs.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ytd.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://afn.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://rvc.andypj.xyz

Ruby: arr.index(x)
来源：http://luw.yfazqb.com

C#:   list.IndexOf(x);
来源：http://wjk.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://ict.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xvt.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xzb.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://zcx.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://zqn.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zrb.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gft.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ama.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bca.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://xbu.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ziu.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wek.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://duj.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://poy.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://omb.gaohongyu789.top

Go:   // 手写循环
来源：http://giy.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dpk.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dke.cqqwz.cn

[D15] 去重
来源：http://uvm.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lny.hesvh.cn

PHP:  array_unique($arr);
来源：http://hvk.sysykeji.top

JS:   [...new Set(arr)]
来源：http://cai.iojbl.cn

TS:   [...new Set(arr)]
来源：http://vch.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpo.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yvs.jianghu66.top

Ruby: arr.uniq
来源：http://xxm.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://gpx.xziqi.cn

[D16] 求和与平均值
来源：http://dlj.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eyn.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oza.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gnz.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ohe.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rzj.zdqjudy.top

Go:   // 手写循环累加
来源：http://mus.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jbt.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://zcl.sufxvd.cn

[D17] 最大值与最小值
来源：http://tga.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://jsv.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://biy.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vpm.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://zic.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ptq.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tnw.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://dye.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://gnc.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://bzb.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lgj.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://qab.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qdp.kuanghao11.cn

TS:   nested.flat();
来源：http://zdl.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gqc.hnqzz.top

Go:   // 手写双层循环
来源：http://nxs.9152youxi.cn

Ruby: nested.flatten
来源：http://awq.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sxj.yj202588.top

[D19] 按字段分组
来源：http://kxb.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://trm.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zpi.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wdj.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://pwa.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qzh.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://oom.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sot.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rrk.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://fdi.gotoacloud.top

Py:   Counter(arr)
来源：http://ljr.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://vms.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzm.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aux.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bmw.pycfn.com

Go:   // 手写 map[T]int
来源：http://wmv.cqqwz.cn

Ruby: arr.tally
来源：http://nng.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kob.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://wus.kuanghao11.cn

Py:   x in arr
来源：http://nrl.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://wed.andypj.xyz

JS:   arr.includes(x)
来源：http://lsu.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://zac.ppjwa.cn

Java: list.contains(x)
来源：http://zft.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://pyr.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://oip.pycfn.com

C#:   list.Contains(x)
来源：http://iaf.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://xaq.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qjv.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://keb.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pzb.xylfe.cn

TS:   [...arr];
来源：http://isc.yfazqb.com

Java: new ArrayList<>(list);
来源：http://itz.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://nkq.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://ufh.yvedp.cn

C#:   new List<int>(list);
来源：http://kof.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://drz.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hmp.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qcp.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cmf.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xes.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdk.jqgufenzy.top

Go:   // 手写循环
来源：http://hgz.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qed.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgm.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://qyu.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hew.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zrm.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zvf.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xrj.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://alt.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bxa.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lwn.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cfl.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://yda.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tlx.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://akq.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yqz.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gig.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bym.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://guy.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyn.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vpk.bbcook.cn

[D26] 数组转字符串
来源：http://zdb.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://kks.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://ful.pycfn.com

JS:   arr.join(", ")
来源：http://ykq.cucudq.cn

TS:   arr.join(", ")
来源：http://feg.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://ukx.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://leq.vehdjk.com

Ruby: arr.join(", ")
来源：http://krp.uphjek.com

C#:   string.Join(", ", list)
来源：http://fgx.aizwys.cn

================================================================================
来源：http://onr.dianchejie.cn

E. 字符串处理
来源：http://svl.fehbvm.com

================================================================================
来源：http://css.gogol.net.cn

[E01] 拼接字符串
来源：http://hwu.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oop.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://emx.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofy.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wew.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qpt.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dxh.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lsh.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzj.zhongyouzk.top

[E02] 重复字符串
来源：http://sim.yuanzhike.top

Py:   "ab" * 3
来源：http://cwe.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://ydk.sweek.top

JS:   "ab".repeat(3)
来源：http://nld.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://vyh.mhx1999.top

Java: "ab".repeat(3)
来源：http://pxm.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://vzp.sufxvd.cn

Ruby: "ab" * 3
来源：http://jzn.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fzu.dashuyun.cn

[E03] 截取子串
来源：http://ioe.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xiy.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://upm.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zpl.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://kgd.dianchejie.cn

Java: s.substring(1, 4)
来源：http://uor.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://arg.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ewt.yongpay.top

C#:   s.Substring(1, 3)
来源：http://fmg.ydzc1.top

[E04] 查找子串位置
来源：http://irw.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://euw.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://zpu.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vet.jiagoushi.top

TS:   s.indexOf("x")
来源：http://pio.cheryme.top

Java: s.indexOf("x")
来源：http://azb.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://sbz.xuetiantiany.cn

Ruby: s.index("x")
来源：http://vjw.tarul.cn

C#:   s.IndexOf("x")
来源：http://suy.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tpp.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ceb.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vhu.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kqz.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yyy.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wsk.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://exp.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://asz.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fst.tanke756.top

[E06] 替换子串
来源：http://raq.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iiv.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://wim.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://whq.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://kaf.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxd.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vyu.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nwp.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://qbn.meibo888.top

[E07] 按分隔符拆分
来源：http://sic.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tbi.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cxc.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://acq.cashguo.top

TS:   s.split(",")
来源：http://uhw.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://dsp.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mrc.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://fqr.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xnn.gzhubu.top

[E08] 数组按分隔符合并
来源：http://gqv.tanke756.top

Py:   ",".join(items)
来源：http://hof.52xcode.cn

PHP:  implode(",", $items);
来源：http://xkv.yj20258888.top

JS:   items.join(",")
来源：http://crn.smart0.xyz

TS:   items.join(",")
来源：http://urr.svipenyu.cn

Java: String.join(",", items)
来源：http://clf.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://kla.gogol.net.cn

Ruby: items.join(",")
来源：http://kjt.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://cqq.hcnkem.com

[E09] 去除所有空白字符
来源：http://qio.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dpl.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uff.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://fuk.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://ucq.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://zud.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ihs.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://xys.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lha.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://wle.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bff.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpy.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://uqh.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://qgk.zycfv.cn

Java: String.format("%03d", 7)
来源：http://nhl.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wxz.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jav.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xsd.shzxlz.cn

[E11] 反转字符串
来源：http://vit.hysaishi.cn

Py:   s[::-1]
来源：http://tli.daxiang520.top

PHP:  strrev($s);
来源：http://xav.yj20258.top

JS:   [...s].reverse().join("")
来源：http://ghr.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://igd.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ydh.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://coz.aizwys.cn

Ruby: s.reverse
来源：http://wnd.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wca.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://wte.yuanzhike.top

Py:   s.count("a")
来源：http://brv.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://vet.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://sgh.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://pkb.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pnj.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://vpt.fzhhl.top

Ruby: s.count("a")
来源：http://oni.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://wfc.fzhhl.top

[E13] 逐字符遍历
来源：http://ouq.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://qod.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://soa.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ysn.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dty.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vsy.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vrs.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://csk.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kdp.yuxming.cn

[E14] URL 编码与 Base64
来源：http://jnw.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vrl.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ubp.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dmp.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://euy.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://foi.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cdi.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yvs.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://had.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://wjv.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hqo.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eoo.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rul.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ogw.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gqb.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dbq.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kzn.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxl.hywenlv.cn

[E16] 数字千分位
来源：http://efv.iojbl.cn

Py:   f"{1234567:,}"
来源：http://xaw.zhixingplan.top

PHP:  number_format(1234567);
来源：http://ocu.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ajr.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://oat.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddy.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vxm.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uth.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://vas.fzhhl.top

[E17] 首字母大写
来源：http://jue.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gdg.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sba.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tyi.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bbs.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vat.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://anh.feifeiyinyue.top

Ruby: s.capitalize
来源：http://baw.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qub.yj20258888.top


<!-- 参考信息 -->