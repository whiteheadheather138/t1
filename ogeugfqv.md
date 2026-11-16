代发 wailian999

[D11] 反转数组
来源：http://vcg.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qhk.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://wqq.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zur.tianlin.xyz

TS:   [...arr].reverse();
来源：http://lji.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://fid.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://ztx.sxryk.cn

Ruby: arr.reverse
来源：http://joj.wangdashe.top

C#:   list.Reverse();
来源：http://yvb.daria6918.cn

[D12] 查找元素下标
来源：http://jag.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://pnk.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vyq.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jch.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rtu.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hmj.hammf.cn

Go:   slices.Index(arr, x)
来源：http://qij.yongpay.top

Ruby: arr.index(x)
来源：http://ehs.havefunace.top

C#:   list.IndexOf(x);
来源：http://fce.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://nsi.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bzv.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fvo.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://szd.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://znu.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyv.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hxb.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bpr.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://coi.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://bmd.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yml.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yhr.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://sxs.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://bvf.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://guz.hammf.cn

Go:   // 手写循环
来源：http://wpm.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iij.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ler.andypj.xyz

[D15] 去重
来源：http://tzb.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rvo.yuxming.cn

PHP:  array_unique($arr);
来源：http://cgj.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://hij.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://ydd.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lyf.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://quj.xylfe.cn

Ruby: arr.uniq
来源：http://sbw.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://dzj.xuetiantiany.cn

[D16] 求和与平均值
来源：http://din.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gez.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gij.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bwz.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yve.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cfb.jqgufenzy.top

Go:   // 手写循环累加
来源：http://dcu.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wps.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://cmo.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://dlb.birdmap.top

Py:   max(arr);  min(arr)
来源：http://val.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://nuy.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ljm.dianchejie.cn

TS:   Math.max(...arr);
来源：http://fsj.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://klc.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pqh.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://qip.hammf.cn

C#:   list.Max();  list.Min()
来源：http://xrz.pycfn.com

[D18] 扁平化嵌套数组
来源：http://hpz.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zsx.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://kbb.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jwm.gogol.net.cn

TS:   nested.flat();
来源：http://fzs.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xdh.yangfankeji.com

Go:   // 手写双层循环
来源：http://ili.kuanghao11.cn

Ruby: nested.flatten
来源：http://tcf.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jdi.zdbjq.cn

[D19] 按字段分组
来源：http://xjn.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wta.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lns.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bwb.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://svx.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eiz.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://hjo.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://tes.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lbe.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://twe.jianghu66.top

Py:   Counter(arr)
来源：http://vqi.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://bvz.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhu.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://air.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wxi.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://hkn.bjfxy.top

Ruby: arr.tally
来源：http://stx.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aio.316326.xyz

[D21] 判断是否包含某元素
来源：http://wnw.zycfv.cn

Py:   x in arr
来源：http://hzr.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://ppi.zdbjq.cn

JS:   arr.includes(x)
来源：http://qbt.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://rlt.yonumen.top

Java: list.contains(x)
来源：http://kfi.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://hhm.xziqi.cn

Ruby: arr.include?(x)
来源：http://ohv.guowangkeji.top

C#:   list.Contains(x)
来源：http://fxh.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://tyf.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eml.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://luc.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uzc.cashguo.top

TS:   [...arr];
来源：http://jdx.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://xrx.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://kpj.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://oeh.andypj.xyz

C#:   new List<int>(list);
来源：http://blc.xinyue.icu

[D23] reduce 累积计算
来源：http://rgy.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqw.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vho.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://taf.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gou.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qoo.guowangkeji.top

Go:   // 手写循环
来源：http://uvr.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jqy.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lvh.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://zyl.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pob.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hqe.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://frn.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hgc.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aed.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vqp.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://por.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mzq.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://qww.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fks.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://igc.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jlt.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pxh.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fsx.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tyl.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fbt.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gvn.0kj1m.cn

[D26] 数组转字符串
来源：http://cch.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://sll.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://bko.cheryme.top

JS:   arr.join(", ")
来源：http://mbs.gzhubu.top

TS:   arr.join(", ")
来源：http://vcd.yuanzhike.top

Java: String.join(", ", list)
来源：http://org.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://mig.cucudq.cn

Ruby: arr.join(", ")
来源：http://eiq.ybcxt.top

C#:   string.Join(", ", list)
来源：http://veu.shanyushiyangtech.top

================================================================================
来源：http://jyi.quarkkingdee.top

E. 字符串处理
来源：http://xng.dianchejie.cn

================================================================================
来源：http://bnu.hesvh.cn

[E01] 拼接字符串
来源：http://umj.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vel.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zgw.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqr.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejv.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nhb.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lmd.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ett.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rsg.hnqzz.top

[E02] 重复字符串
来源：http://ufn.zhixingplan.top

Py:   "ab" * 3
来源：http://hvg.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://ajq.epnwcf.com

JS:   "ab".repeat(3)
来源：http://lft.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://wex.ehwqpu.com

Java: "ab".repeat(3)
来源：http://fnf.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://mfk.cqqwz.cn

Ruby: "ab" * 3
来源：http://yup.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://icf.xylfe.cn

[E03] 截取子串
来源：http://owt.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://epw.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://izw.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ipq.tian-w.cn

TS:   s.slice(1, 4)
来源：http://zeb.redwolf501.top

Java: s.substring(1, 4)
来源：http://mae.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://srb.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mhb.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://uxb.jiagoushi.top

[E04] 查找子串位置
来源：http://hji.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://gxr.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://log.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dzk.hammf.cn

TS:   s.indexOf("x")
来源：http://rog.yongpay.top

Java: s.indexOf("x")
来源：http://hqp.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://dma.jqgufenzy.top

Ruby: s.index("x")
来源：http://lrs.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://qqd.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://emi.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ixt.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sjq.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://onc.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://jva.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lgu.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fkl.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ewl.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jwp.sysykeji.top

[E06] 替换子串
来源：http://nrs.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cst.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://ztc.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbb.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://ntd.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ico.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zyf.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tfb.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://gew.vehdjk.com

[E07] 按分隔符拆分
来源：http://wkz.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xcz.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://erz.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qke.zhengqikj.top

TS:   s.split(",")
来源：http://rvg.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://vfe.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kxi.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://gzr.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vbx.uphjek.com

[E08] 数组按分隔符合并
来源：http://mdq.jqgufenzy.top

Py:   ",".join(items)
来源：http://orx.ivvv.top

PHP:  implode(",", $items);
来源：http://efo.ehwqpu.com

JS:   items.join(",")
来源：http://fej.zhixingplan.top

TS:   items.join(",")
来源：http://lko.vqdsnc.cn

Java: String.join(",", items)
来源：http://cat.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://mcm.chenlongwang.top

Ruby: items.join(",")
来源：http://cuh.ppjwa.cn

C#:   string.Join(",", items)
来源：http://mhx.gogol.net.cn

[E09] 去除所有空白字符
来源：http://kzx.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://apv.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pnn.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://ygq.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://jsp.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://inb.wangshuangyany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jgl.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hqp.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qhr.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://qft.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://arx.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vjy.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://fch.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://ddy.mhx1999.top

Java: String.format("%03d", 7)
来源：http://ryf.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dec.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovb.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ptg.sysykeji.top

[E11] 反转字符串
来源：http://upd.daxiang520.top

Py:   s[::-1]
来源：http://txe.cheryme.top

PHP:  strrev($s);
来源：http://lcr.birdmap.top

JS:   [...s].reverse().join("")
来源：http://yem.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://rjt.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wfb.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ouo.shanyushiyangtech.top

Ruby: s.reverse
来源：http://rbw.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://fab.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://vgc.cashguo.top

Py:   s.count("a")
来源：http://lyl.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://ilu.cucudq.cn

JS:   s.split("a").length - 1
来源：http://xyq.c1oappe.top

TS:   s.split("a").length - 1
来源：http://rcb.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://owo.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://elz.tian-w.cn

Ruby: s.count("a")
来源：http://odo.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://usp.yj20258.top

[E13] 逐字符遍历
来源：http://ezw.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://uyy.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wkd.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ocn.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvf.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tdc.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://duu.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yvh.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mnx.yuxming.cn

[E14] URL 编码与 Base64
来源：http://hns.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gmv.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jco.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nii.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://alu.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fsu.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nqb.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wpa.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://chj.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://ksi.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hfg.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://stu.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://unt.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ytm.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gxa.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xlw.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hyz.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zkk.zycfv.cn

[E16] 数字千分位
来源：http://lmk.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://yuk.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://ihz.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fea.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wnl.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rkr.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fat.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxa.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://don.meibo888.top

[E17] 首字母大写
来源：http://bzg.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fct.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gxf.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjo.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djz.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vvl.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zng.jianghu66.top

Ruby: s.capitalize
来源：http://mqp.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rnt.chenlongwang.top


<!-- 参考信息 -->