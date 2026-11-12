代发 wailian999

TS:   [...arr].reverse();
来源：http://fvp.snrcjt.cn

Java: Collections.reverse(list);
来源：http://qtc.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://mvs.gogol.net.cn

Ruby: arr.reverse
来源：http://ycm.nanxinkj.top

C#:   list.Reverse();
来源：http://tol.ivvv.top

[D12] 查找元素下标
来源：http://bfi.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://vaf.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hzf.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dwl.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cmr.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsb.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://kbt.gzhubu.top

Ruby: arr.index(x)
来源：http://jri.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://ern.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://sis.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bya.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wvi.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://tdp.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://tsr.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjb.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vwm.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://pwm.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jcr.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://jzb.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zxu.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqx.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://ser.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://wfu.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvg.cucudq.cn

Go:   // 手写循环
来源：http://mug.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ife.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zoo.sxryk.cn

[D15] 去重
来源：http://cnm.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lhv.andypj.xyz

PHP:  array_unique($arr);
来源：http://abo.yj20258.top

JS:   [...new Set(arr)]
来源：http://zdv.yfazqb.com

TS:   [...new Set(arr)]
来源：http://zjo.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sls.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://pnb.sufxvd.cn

Ruby: arr.uniq
来源：http://bkp.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://flx.iojbl.cn

[D16] 求和与平均值
来源：http://cnu.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hch.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mvr.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ors.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgm.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://faf.gotoacloud.top

Go:   // 手写循环累加
来源：http://btx.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gku.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://bwd.hywenlv.cn

[D17] 最大值与最小值
来源：http://uil.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://yhe.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://qqh.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rru.daxiang520.top

TS:   Math.max(...arr);
来源：http://wnv.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rxz.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yrt.316326.xyz

Ruby: arr.max;  arr.min
来源：http://ril.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://lii.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://nby.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aso.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://rrl.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uuk.pycfn.com

TS:   nested.flat();
来源：http://esi.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://frt.yuxming.cn

Go:   // 手写双层循环
来源：http://jqo.jqgufenzy.top

Ruby: nested.flatten
来源：http://are.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://znk.ivvv.top

[D19] 按字段分组
来源：http://pbp.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oxx.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://crw.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lcr.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cte.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dov.yonumen.top

Go:   // 手写 map[string][]T
来源：http://hgj.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ynv.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wfv.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://bfo.haohaochexian.top

Py:   Counter(arr)
来源：http://xci.uphjek.com

PHP:  array_count_values($arr);
来源：http://cfc.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xrh.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://obd.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sux.xinyue.icu

Go:   // 手写 map[T]int
来源：http://bur.yj202588.top

Ruby: arr.tally
来源：http://xhp.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jrz.yj202588.top

[D21] 判断是否包含某元素
来源：http://ydb.hfpthk.cn

Py:   x in arr
来源：http://spe.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://qvv.yuxming.cn

JS:   arr.includes(x)
来源：http://myu.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://lmh.daxiang520.top

Java: list.contains(x)
来源：http://wla.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://nxq.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://uuh.zdbjq.cn

C#:   list.Contains(x)
来源：http://glf.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://viv.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aoo.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gur.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xjn.aibaodan.cn

TS:   [...arr];
来源：http://kbd.hcnkem.com

Java: new ArrayList<>(list);
来源：http://qpr.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://lqa.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://krw.nwbrower.top

C#:   new List<int>(list);
来源：http://cwf.wangdashe.top

[D23] reduce 累积计算
来源：http://ezu.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bjs.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mhh.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kib.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rkc.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sli.tianlin.xyz

Go:   // 手写循环
来源：http://lyc.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xbc.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://psj.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://ylk.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tmj.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ous.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ngl.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cek.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wtb.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bbu.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://piq.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gzn.316326.xyz

[D25] Set 集合去重与交并差
来源：http://jke.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sud.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xlo.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vfs.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yle.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hzz.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vtm.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oow.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qdi.jlsjyb.cn

[D26] 数组转字符串
来源：http://spa.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://xuw.sweek.top

PHP:  implode(", ", $arr);
来源：http://psc.cucudq.cn

JS:   arr.join(", ")
来源：http://ybm.hammf.cn

TS:   arr.join(", ")
来源：http://lop.meibo888.top

Java: String.join(", ", list)
来源：http://bzr.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://wlm.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://rac.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://bfp.hesvh.cn

================================================================================
来源：http://cct.sweek.top

E. 字符串处理
来源：http://ynr.ydjk.org.cn

================================================================================
来源：http://fur.tanke756.top

[E01] 拼接字符串
来源：http://unl.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdy.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xgb.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bts.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lwv.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cdm.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ued.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mos.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wui.nanxinkj.top

[E02] 重复字符串
来源：http://noj.hysaishi.cn

Py:   "ab" * 3
来源：http://zrs.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://jdz.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://vak.sxryk.cn

TS:   "ab".repeat(3)
来源：http://ttg.sysykeji.top

Java: "ab".repeat(3)
来源：http://cnk.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://zhv.zhengqikj.top

Ruby: "ab" * 3
来源：http://ydz.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qvo.jinqigfzy.top

[E03] 截取子串
来源：http://puy.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cze.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://amg.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yxe.316326.xyz

TS:   s.slice(1, 4)
来源：http://yfr.yuanzhike.top

Java: s.substring(1, 4)
来源：http://hpy.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lmt.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://bka.hammf.cn

C#:   s.Substring(1, 3)
来源：http://wxo.sysykeji.top

[E04] 查找子串位置
来源：http://bxa.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://oug.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://hfh.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eeh.hfpthk.cn

TS:   s.indexOf("x")
来源：http://dks.ybcxt.top

Java: s.indexOf("x")
来源：http://uzt.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://wma.snrcjt.cn

Ruby: s.index("x")
来源：http://nwg.fehbvm.com

C#:   s.IndexOf("x")
来源：http://otl.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gyo.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://njf.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mzz.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://occ.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zld.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zfr.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezi.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mkv.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://exg.hcnkem.com

[E06] 替换子串
来源：http://dax.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yay.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://zql.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vby.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://dph.cqqwz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jct.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jgv.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nnp.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://twh.gzhubu.top

[E07] 按分隔符拆分
来源：http://qej.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pjn.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ipz.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://cty.cheryme.top

TS:   s.split(",")
来源：http://xwy.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://hcc.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eqh.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://owc.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uyj.pycfn.com

[E08] 数组按分隔符合并
来源：http://ujs.svipenyu.cn

Py:   ",".join(items)
来源：http://dxa.quarkkingdee.top

PHP:  implode(",", $items);
来源：http://zui.pycfn.com

JS:   items.join(",")
来源：http://rrc.jiagoushi.top

TS:   items.join(",")
来源：http://pfh.sysykeji.top

Java: String.join(",", items)
来源：http://okp.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://fho.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://xmj.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://bdn.jianghu66.top

[E09] 去除所有空白字符
来源：http://zox.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lyk.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sxy.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://wix.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://pml.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://cpz.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tcg.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zew.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lpz.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://ikh.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vyy.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rlv.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://yzx.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://ais.meibo888.top

Java: String.format("%03d", 7)
来源：http://jth.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://stt.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nrz.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzk.dashuyun.cn

[E11] 反转字符串
来源：http://kqm.ybcxt.top

Py:   s[::-1]
来源：http://zlw.52xcode.cn

PHP:  strrev($s);
来源：http://enx.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://htg.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://cqi.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dxs.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xlz.vqdsnc.cn

Ruby: s.reverse
来源：http://jxi.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://ray.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://bnd.cashguo.top

Py:   s.count("a")
来源：http://lgo.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://opr.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://wkt.fengsongda.top

TS:   s.split("a").length - 1
来源：http://cgz.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gxe.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://kxf.52xcode.cn

Ruby: s.count("a")
来源：http://slz.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://iyc.ydzc1.top

[E13] 逐字符遍历
来源：http://asg.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://yyn.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yeg.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://hlk.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://orp.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xqm.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aqr.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zqf.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://won.yonumen.top

[E14] URL 编码与 Base64
来源：http://och.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ppw.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nre.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ufy.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vwq.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blj.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bna.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wvo.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dge.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://smy.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://gvv.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dim.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tfn.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://qog.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zkd.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tjm.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmh.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wcb.jqgfzy.top

[E16] 数字千分位
来源：http://ijy.andypj.xyz

Py:   f"{1234567:,}"
来源：http://xsr.yonumen.top

PHP:  number_format(1234567);
来源：http://gvt.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tzo.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://tux.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sgw.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qky.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wuy.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://idh.yj202588.top

[E17] 首字母大写
来源：http://vfu.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vpw.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aly.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ckj.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jrk.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eiq.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dri.iojbl.cn

Ruby: s.capitalize
来源：http://gpl.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wpv.hywenlv.cn

[E18] 模板占位符替换
来源：http://jwi.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lrk.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mjc.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://gdp.cdnleiting.top


<!-- 参考信息 -->