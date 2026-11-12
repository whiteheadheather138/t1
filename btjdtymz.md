代发 wailian999

[D11] 反转数组
来源：http://cxt.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://znq.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://izg.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wtl.daria6918.cn

TS:   [...arr].reverse();
来源：http://ftk.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://sua.havefunace.top

Go:   slices.Reverse(arr)
来源：http://hmo.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://ffb.nanxuanxn.top

C#:   list.Reverse();
来源：http://rpf.gaohongyu789.top

[D12] 查找元素下标
来源：http://rzp.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://bka.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bqg.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cxc.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kes.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ibm.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://qlc.bjfxy.top

Ruby: arr.index(x)
来源：http://wrb.daxiang520.top

C#:   list.IndexOf(x);
来源：http://nlx.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://uko.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bgr.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://urp.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://oon.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://vyk.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ror.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tdy.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sls.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://stx.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://buw.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ufk.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xzy.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://tas.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://xez.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zjh.sufxvd.cn

Go:   // 手写循环
来源：http://jbo.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://acb.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hrp.bjfxy.top

[D15] 去重
来源：http://sxm.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tuc.jiagoushi.top

PHP:  array_unique($arr);
来源：http://fsv.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://tmx.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://tqz.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dtv.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vuk.bbcook.cn

Ruby: arr.uniq
来源：http://mtz.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://ifb.hongshengwenyu.top

[D16] 求和与平均值
来源：http://tei.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rke.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eaj.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wkv.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dyu.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nhe.52xcode.cn

Go:   // 手写循环累加
来源：http://mje.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qwn.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://okd.yanxiufei.cn

[D17] 最大值与最小值
来源：http://bzb.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://apq.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://dlj.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dqp.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://fba.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qwz.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://onu.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://gqx.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://cov.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://bdz.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wib.sweek.top

PHP:  array_merge(...$nested);
来源：http://zon.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uaq.dashuyun.cn

TS:   nested.flat();
来源：http://voh.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aoj.zhongyouzk.top

Go:   // 手写双层循环
来源：http://lrf.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://qgo.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ztn.dianchejie.cn

[D19] 按字段分组
来源：http://bwi.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vdu.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fkh.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bea.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hst.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xcn.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://chm.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bwh.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fnr.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://kmg.xylfe.cn

Py:   Counter(arr)
来源：http://jod.ydzc1.top

PHP:  array_count_values($arr);
来源：http://jfq.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tzm.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzs.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yka.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://tsy.xylfe.cn

Ruby: arr.tally
来源：http://mvt.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://piz.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://mxz.shuidangran.top

Py:   x in arr
来源：http://ksk.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://vrr.ydzc1.top

JS:   arr.includes(x)
来源：http://jdr.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://qwf.nanxuanxn.top

Java: list.contains(x)
来源：http://ngw.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://hkg.meibo888.top

Ruby: arr.include?(x)
来源：http://cxk.meibo888.top

C#:   list.Contains(x)
来源：http://mpm.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://vqz.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qom.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://atv.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rtb.gogol.net.cn

TS:   [...arr];
来源：http://yrf.xziqi.cn

Java: new ArrayList<>(list);
来源：http://ugj.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://rdo.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://cxb.jyoumei.cn

C#:   new List<int>(list);
来源：http://zpy.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://wqd.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qxy.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vfi.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxt.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eet.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://drt.yfazqb.com

Go:   // 手写循环
来源：http://mbd.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkd.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kve.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://hma.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dxf.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xpe.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sqb.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gpg.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rpb.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzo.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ohg.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://axx.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://fek.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dse.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jbs.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dpc.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kuh.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bhe.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pbb.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ncr.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://snn.gotoacloud.top

[D26] 数组转字符串
来源：http://wnf.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://vci.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://uer.zhongyouzk.top

JS:   arr.join(", ")
来源：http://wnw.chenlongwang.top

TS:   arr.join(", ")
来源：http://wdb.guannengcc.top

Java: String.join(", ", list)
来源：http://jim.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://fnr.cqqwz.cn

Ruby: arr.join(", ")
来源：http://jev.ybcxt.top

C#:   string.Join(", ", list)
来源：http://ptm.zhixingplan.top

================================================================================
来源：http://zow.xuanzx.com

E. 字符串处理
来源：http://hgu.nanxuanxn.top

================================================================================
来源：http://anr.vqdsnc.cn

[E01] 拼接字符串
来源：http://bcg.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jud.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fyh.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ynb.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sus.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ixc.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cjh.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtw.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zuv.hnqzz.top

[E02] 重复字符串
来源：http://nvn.hcnkem.com

Py:   "ab" * 3
来源：http://wsl.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://ysx.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://ytr.daxiang520.top

TS:   "ab".repeat(3)
来源：http://bvv.dashuyun.cn

Java: "ab".repeat(3)
来源：http://iro.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://tuu.hammf.cn

Ruby: "ab" * 3
来源：http://nsp.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sdm.fzhhl.top

[E03] 截取子串
来源：http://ejo.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izy.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://osd.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xkj.sweek.top

TS:   s.slice(1, 4)
来源：http://dge.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://aoa.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iby.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://dbp.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://ctj.jyoumei.cn

[E04] 查找子串位置
来源：http://wlk.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://zrj.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://qvp.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zmp.yongpay.top

TS:   s.indexOf("x")
来源：http://qja.kuanghao11.cn

Java: s.indexOf("x")
来源：http://bna.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://svl.xylfe.cn

Ruby: s.index("x")
来源：http://kaq.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://tmm.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rjn.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cjm.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xwm.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://old.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zih.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dua.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://amb.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ers.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvn.yueranfly.top

[E06] 替换子串
来源：http://mpo.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qpo.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://app.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aka.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://ecv.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvc.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://azs.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lnd.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://dfb.sweek.top

[E07] 按分隔符拆分
来源：http://cce.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lnl.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xfw.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tbp.pycfn.com

TS:   s.split(",")
来源：http://yqf.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sdy.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tfk.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://phi.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cbq.redwolf501.top

[E08] 数组按分隔符合并
来源：http://uhz.chenjidiqi.icu

Py:   ",".join(items)
来源：http://ddj.jiagoushi.top

PHP:  implode(",", $items);
来源：http://dyi.sufxvd.cn

JS:   items.join(",")
来源：http://mfe.gogol.net.cn

TS:   items.join(",")
来源：http://dsv.aibaodan.cn

Java: String.join(",", items)
来源：http://kei.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://rks.mhx1999.top

Ruby: items.join(",")
来源：http://rrb.epnwcf.com

C#:   string.Join(",", items)
来源：http://jbu.bbcook.cn

[E09] 去除所有空白字符
来源：http://cgd.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bwz.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yhz.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://hwe.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://xfg.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://qjd.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://urr.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://orj.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://siq.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://wqx.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wyi.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kcf.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://mra.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://lnr.redwolf501.top

Java: String.format("%03d", 7)
来源：http://awl.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wox.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xpf.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lsx.cqqwz.cn

[E11] 反转字符串
来源：http://okx.yangfankeji.com

Py:   s[::-1]
来源：http://ucq.yongpay.top

PHP:  strrev($s);
来源：http://vkz.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://fxc.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://qxx.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://koa.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lzu.zycfv.cn

Ruby: s.reverse
来源：http://ajx.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://fvu.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://gxm.ppjwa.cn

Py:   s.count("a")
来源：http://ybo.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://iwz.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://bpy.bjfxy.top

TS:   s.split("a").length - 1
来源：http://wwj.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vft.meibo888.top

Go:   strings.Count(s, "a")
来源：http://dck.daria6918.cn

Ruby: s.count("a")
来源：http://nlq.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://utm.yj20258888.top

[E13] 逐字符遍历
来源：http://ife.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://htx.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://una.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://nuy.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xdw.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://est.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gbu.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://cpg.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jgu.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://ghj.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gkc.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ieu.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hvb.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qaz.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llh.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uvv.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hcj.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wva.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://efh.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hld.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fag.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yrp.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mef.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ddo.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qpw.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dlm.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mlu.hammf.cn

[E16] 数字千分位
来源：http://vdn.shuidangran.top

Py:   f"{1234567:,}"
来源：http://tqt.daxiang520.top

PHP:  number_format(1234567);
来源：http://jgq.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eos.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://epx.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iax.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uzh.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlp.havefunace.top

C#:   1234567.ToString("N0")
来源：http://qov.ybcxt.top

[E17] 首字母大写
来源：http://zet.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nsw.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://eib.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tdg.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gcp.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jjh.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yxs.gzhubu.top

Ruby: s.capitalize
来源：http://shw.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fex.xingfuxueyuan.xyz


<!-- 参考信息 -->