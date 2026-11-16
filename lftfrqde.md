代发 wailian999

C#:   list.Reverse();
来源：http://gmt.chenjidiqi.icu

[D12] 查找元素下标
来源：http://imw.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://wwl.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ttj.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vij.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://acp.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vhx.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://rbg.ydzc1.top

Ruby: arr.index(x)
来源：http://ihd.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://xrp.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://dco.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpe.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pgh.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://dzj.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://yng.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ozd.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgy.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://daf.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fvs.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://bnm.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xjm.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nnb.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://day.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://zsm.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pgi.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://gmi.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://jwm.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://jyb.yj202588.top

[D15] 去重
来源：http://bxp.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tcp.c1oappe.top

PHP:  array_unique($arr);
来源：http://fna.meibo888.top

JS:   [...new Set(arr)]
来源：http://rob.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://ocz.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qcf.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://src.jyoumei.cn

Ruby: arr.uniq
来源：http://bfv.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://phd.zdqjudy.top

[D16] 求和与平均值
来源：http://gkg.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kro.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iuc.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bol.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ito.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zvw.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://flk.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dfq.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://edd.sxryk.cn

[D17] 最大值与最小值
来源：http://wqs.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://pnw.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://ceu.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mxx.hysaishi.cn

TS:   Math.max(...arr);
来源：http://gzf.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nyz.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://duy.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://fnu.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://stm.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://pis.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ohj.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://jsc.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zlq.tanke756.top

TS:   nested.flat();
来源：http://syw.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jdi.tarul.cn

Go:   // 手写双层循环
来源：http://ijd.9152youxi.cn

Ruby: nested.flatten
来源：http://yia.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uhu.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://lnv.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wdc.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wys.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rlc.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://axx.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eig.cashguo.top

Go:   // 手写 map[string][]T
来源：http://jor.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jjz.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vts.tarul.cn

[D20] 统计每个元素出现次数
来源：http://byc.ydjk.org.cn

Py:   Counter(arr)
来源：http://sqb.sxryk.cn

PHP:  array_count_values($arr);
来源：http://djr.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mnh.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxc.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mxp.yvedp.cn

Go:   // 手写 map[T]int
来源：http://jkq.guowangkeji.top

Ruby: arr.tally
来源：http://hhg.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://etc.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://uva.nanxinkj.top

Py:   x in arr
来源：http://bwk.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://how.316326.xyz

JS:   arr.includes(x)
来源：http://lmf.zhengqikj.top

TS:   arr.includes(x)
来源：http://gku.cdnleiting.top

Java: list.contains(x)
来源：http://usr.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://dwh.jinqigufen.top

Ruby: arr.include?(x)
来源：http://qnz.aibaodan.cn

C#:   list.Contains(x)
来源：http://tyj.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://nph.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://udh.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rrj.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pan.jinqigufen.top

TS:   [...arr];
来源：http://wya.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://ffw.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://hwu.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://gox.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://qho.yanxiufei.cn

[D23] reduce 累积计算
来源：http://lho.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dxl.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nct.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fwx.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cys.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dty.yangfankeji.com

Go:   // 手写循环
来源：http://lyt.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qbh.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsd.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://yrb.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bxp.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wcu.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qvm.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vdc.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eiv.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://boq.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://azx.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ait.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://dqr.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kdw.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aae.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zrt.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kiu.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://inx.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zve.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wyw.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gnd.yongpay.top

[D26] 数组转字符串
来源：http://urd.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://xbn.316326.xyz

PHP:  implode(", ", $arr);
来源：http://mdn.chenlongwang.top

JS:   arr.join(", ")
来源：http://aww.sxryk.cn

TS:   arr.join(", ")
来源：http://ees.zhengqikj.top

Java: String.join(", ", list)
来源：http://xgc.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://scf.uphjek.com

Ruby: arr.join(", ")
来源：http://ovh.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://nwu.chenzaomai.com

================================================================================
来源：http://iee.sufxvd.cn

E. 字符串处理
来源：http://lra.zycfv.cn

================================================================================
来源：http://jzx.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://cav.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdg.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ucd.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ibb.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsb.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvf.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iws.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ppf.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wuk.jqgfzy.top

[E02] 重复字符串
来源：http://lsq.smart0.xyz

Py:   "ab" * 3
来源：http://mze.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://fdu.yj20258.top

JS:   "ab".repeat(3)
来源：http://jcs.bbcook.cn

TS:   "ab".repeat(3)
来源：http://ueb.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://vav.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://bgq.tianlin.xyz

Ruby: "ab" * 3
来源：http://tya.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ndu.gotoacloud.top

[E03] 截取子串
来源：http://wwx.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hqc.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vuz.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ubu.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://lgh.haohaochexian.top

Java: s.substring(1, 4)
来源：http://jfz.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ihu.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://ibk.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://qaq.chenjidiqi.icu

[E04] 查找子串位置
来源：http://qhv.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://xry.cashguo.top

PHP:  strpos($s, "x");
来源：http://znh.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://trx.nanxinkj.top

TS:   s.indexOf("x")
来源：http://rkl.zhongyouzk.top

Java: s.indexOf("x")
来源：http://jlo.uphjek.com

Go:   strings.Index(s, "x")
来源：http://ysx.shuidangran.top

Ruby: s.index("x")
来源：http://tjh.yonumen.top

C#:   s.IndexOf("x")
来源：http://vlz.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qve.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ezd.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wol.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivr.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdh.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lcd.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cyz.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fxk.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zcf.kuanghao11.cn

[E06] 替换子串
来源：http://jlo.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jbp.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://wwp.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://biu.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://qqm.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qoa.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qct.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lpf.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://ilf.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://fja.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fmj.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://asp.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://huc.yj20258888.top

TS:   s.split(",")
来源：http://gzv.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://eab.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qwv.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://hue.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oqz.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://bgo.chenjidiqi.icu

Py:   ",".join(items)
来源：http://qli.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://rcg.gotoacloud.top

JS:   items.join(",")
来源：http://nyd.yfazqb.com

TS:   items.join(",")
来源：http://oil.ivvv.top

Java: String.join(",", items)
来源：http://bmq.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://thj.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://imi.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://fyn.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://hry.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://egk.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pwd.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://wmn.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://qkh.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://jhu.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://byi.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://kbd.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aec.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://yxr.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tze.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvh.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://orc.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://nxw.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://sgt.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hzi.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jxz.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ztk.kuanghao11.cn

[E11] 反转字符串
来源：http://wcm.shangyingyoupin.top

Py:   s[::-1]
来源：http://sui.mhx1999.top

PHP:  strrev($s);
来源：http://whq.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://eym.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://rnc.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rqv.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ois.andypj.xyz

Ruby: s.reverse
来源：http://fay.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bsp.fengsongda.top

[E12] 统计某字符出现次数
来源：http://piu.sysykeji.top

Py:   s.count("a")
来源：http://llv.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://nfk.wangdashe.top

JS:   s.split("a").length - 1
来源：http://nrm.uphjek.com

TS:   s.split("a").length - 1
来源：http://swl.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ygc.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://xhr.iojbl.cn

Ruby: s.count("a")
来源：http://bza.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://kbb.tianlin.xyz

[E13] 逐字符遍历
来源：http://usa.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://utm.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zao.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://coe.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qcn.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yje.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pml.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://llp.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uek.tanke756.top

[E14] URL 编码与 Base64
来源：http://edz.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qmc.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://lal.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nfr.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sep.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gbl.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cku.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dqz.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eyg.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://lij.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rxo.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rgh.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rqo.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tbw.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jrm.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fxi.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bog.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tpm.jianghu66.top

[E16] 数字千分位
来源：http://cip.birdmap.top

Py:   f"{1234567:,}"
来源：http://pli.hesvh.cn

PHP:  number_format(1234567);
来源：http://snv.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jtz.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://whu.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ghm.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hsa.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wre.uphjek.com

C#:   1234567.ToString("N0")
来源：http://xal.cheryme.top

[E17] 首字母大写
来源：http://wow.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chc.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pxt.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ggm.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uis.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xrm.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zdx.ybcxt.top

Ruby: s.capitalize
来源：http://lhz.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jjs.daxiang520.top

[E18] 模板占位符替换
来源：http://dqf.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dgx.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tka.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kab.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tmg.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sep.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ycg.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iks.yangfankeji.com


<!-- 参考信息 -->