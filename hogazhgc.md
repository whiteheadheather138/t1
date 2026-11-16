代发 wailian999

[D11] 反转数组
来源：http://qpf.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gfo.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://iyp.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bof.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://xsa.redwolf501.top

Java: Collections.reverse(list);
来源：http://kfi.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://lbv.ehwqpu.com

Ruby: arr.reverse
来源：http://faz.cashguo.top

C#:   list.Reverse();
来源：http://dwg.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://btm.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://zge.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ueo.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ucl.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zof.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://atv.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://oqs.nanxuanxn.top

Ruby: arr.index(x)
来源：http://sht.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://san.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://dla.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://scn.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wpn.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://hjm.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://fep.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lse.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zxc.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://nay.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://epr.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://spb.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oss.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://khw.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://rbq.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://faz.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yyb.jiagoushi.top

Go:   // 手写循环
来源：http://the.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://oog.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pgm.fengsongda.top

[D15] 去重
来源：http://zhb.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cto.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://uep.ydzc1.top

JS:   [...new Set(arr)]
来源：http://zbv.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://vyg.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eua.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://gcn.hongshengwenyu.top

Ruby: arr.uniq
来源：http://lfs.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://wwt.hysaishi.cn

[D16] 求和与平均值
来源：http://ktg.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gva.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yvz.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ias.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://del.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://joe.bjfxy.top

Go:   // 手写循环累加
来源：http://dkn.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tyo.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://gqj.yuanzhike.top

[D17] 最大值与最小值
来源：http://lgw.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://brj.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://etc.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cek.gotoacloud.top

TS:   Math.max(...arr);
来源：http://nrk.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ooz.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lsr.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://xhi.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://yfu.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://zay.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rro.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://nqo.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wmf.yvedp.cn

TS:   nested.flat();
来源：http://csg.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dcj.0kj1m.cn

Go:   // 手写双层循环
来源：http://yuh.c1oappe.top

Ruby: nested.flatten
来源：http://hjf.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kdd.jyoumei.cn

[D19] 按字段分组
来源：http://oxc.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mns.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eqn.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gki.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://smd.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rzu.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://bia.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://waf.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rct.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://fyl.tian-w.cn

Py:   Counter(arr)
来源：http://mrx.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://aga.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhx.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kcu.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dmz.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://wyv.ivvv.top

Ruby: arr.tally
来源：http://ksq.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qwi.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://ock.ppjwa.cn

Py:   x in arr
来源：http://nxk.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://nyz.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://jni.nwbrower.top

TS:   arr.includes(x)
来源：http://vcg.pengpengdd.cyou

Java: list.contains(x)
来源：http://qog.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://zxj.yuanzhike.top

Ruby: arr.include?(x)
来源：http://vov.hywenlv.cn

C#:   list.Contains(x)
来源：http://gin.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://sld.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://idz.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bfu.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bnw.cheryme.top

TS:   [...arr];
来源：http://klt.52xcode.cn

Java: new ArrayList<>(list);
来源：http://lsd.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://odd.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://hpq.nanxinkj.top

C#:   new List<int>(list);
来源：http://yvx.gaohongyu789.top

[D23] reduce 累积计算
来源：http://xqx.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcs.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cug.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xup.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aoi.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gdh.meibo888.top

Go:   // 手写循环
来源：http://tev.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nie.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdl.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://oac.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ejj.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ije.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cti.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbc.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eeq.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iju.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yve.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wah.sweek.top

[D25] Set 集合去重与交并差
来源：http://lgl.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lrr.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dev.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lwq.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fiw.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xwh.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zts.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oze.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://met.wangshuangyany.cn

[D26] 数组转字符串
来源：http://bcj.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://qjv.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://ovg.haohaochexian.top

JS:   arr.join(", ")
来源：http://vnj.jqgfzy.top

TS:   arr.join(", ")
来源：http://awz.hfpthk.cn

Java: String.join(", ", list)
来源：http://rew.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://qmf.zhixingplan.top

Ruby: arr.join(", ")
来源：http://gkl.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://oke.iojbl.cn

================================================================================
来源：http://iti.wangshuangyany.cn

E. 字符串处理
来源：http://xjl.cashguo.top

================================================================================
来源：http://ftt.dianchejie.cn

[E01] 拼接字符串
来源：http://wsx.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pri.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ulc.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pdt.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwr.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pso.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vvu.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gvm.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vcl.yj20258888.top

[E02] 重复字符串
来源：http://vnr.yueranfly.top

Py:   "ab" * 3
来源：http://xxw.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://wny.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://qyy.yonumen.top

TS:   "ab".repeat(3)
来源：http://alm.ydzc1.top

Java: "ab".repeat(3)
来源：http://rpa.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://nsr.tianlin.xyz

Ruby: "ab" * 3
来源：http://khx.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jjx.pycfn.com

[E03] 截取子串
来源：http://ant.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cto.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hop.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvk.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://kvu.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://nbm.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dek.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://ido.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://nqq.zdbjq.cn

[E04] 查找子串位置
来源：http://rqj.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://aei.jianghu66.top

PHP:  strpos($s, "x");
来源：http://mei.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sxe.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://obi.andypj.xyz

Java: s.indexOf("x")
来源：http://xix.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://tgm.aizwys.cn

Ruby: s.index("x")
来源：http://glp.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://tny.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ayz.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ohd.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hby.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgk.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dmy.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rwb.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dal.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aks.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wca.0kj1m.cn

[E06] 替换子串
来源：http://pip.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cex.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://rgl.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdr.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://kgm.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mew.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vqs.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vtu.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://ycv.yfazqb.com

[E07] 按分隔符拆分
来源：http://wrd.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivh.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vot.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dcw.tian-w.cn

TS:   s.split(",")
来源：http://zgv.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://njw.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gyf.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://ysm.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rrk.ybcxt.top

[E08] 数组按分隔符合并
来源：http://uhh.vehdjk.com

Py:   ",".join(items)
来源：http://vce.yj20258888.top

PHP:  implode(",", $items);
来源：http://sww.xziqi.cn

JS:   items.join(",")
来源：http://kec.sysykeji.top

TS:   items.join(",")
来源：http://cva.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://mec.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://qzh.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://glo.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://zls.cucudq.cn

[E09] 去除所有空白字符
来源：http://djn.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ccz.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fog.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://qzl.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://qgi.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://ggh.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wes.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://mbl.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dly.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://qhq.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jyi.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uja.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://bdm.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://vcu.ivvv.top

Java: String.format("%03d", 7)
来源：http://aby.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uxa.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ivz.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rms.ivvv.top

[E11] 反转字符串
来源：http://dwp.fzhhl.top

Py:   s[::-1]
来源：http://gdp.sufxvd.cn

PHP:  strrev($s);
来源：http://jqq.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://led.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://wga.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bsh.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://odo.yueranfly.top

Ruby: s.reverse
来源：http://smr.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oyy.pycfn.com

[E12] 统计某字符出现次数
来源：http://ylf.nanxinkj.top

Py:   s.count("a")
来源：http://mvn.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://bpd.fktsv.cn

JS:   s.split("a").length - 1
来源：http://cbe.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://zwd.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ino.havefunace.top

Go:   strings.Count(s, "a")
来源：http://kdv.zycfv.cn

Ruby: s.count("a")
来源：http://prc.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://lns.fengsongda.top

[E13] 逐字符遍历
来源：http://qen.pycfn.com

Py:   for ch in s: print(ch)
来源：http://lvl.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dcb.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yhy.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tnr.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vir.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tpo.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tuw.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kuc.tanke756.top

[E14] URL 编码与 Base64
来源：http://pma.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cqj.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://imq.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://okd.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kvv.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yrx.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ari.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jct.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aex.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://ocn.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://raa.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://whl.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nfr.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nwf.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tcq.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bsl.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rrq.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rcg.ybcxt.top

[E16] 数字千分位
来源：http://dhi.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://ipw.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://btb.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ohs.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://epw.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cnm.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vyb.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhu.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://vxp.ivvv.top

[E17] 首字母大写
来源：http://ohj.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vit.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zdo.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://grg.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vcr.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qqa.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ybw.hywenlv.cn

Ruby: s.capitalize
来源：http://wmi.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zrw.zycfv.cn


<!-- 参考信息 -->