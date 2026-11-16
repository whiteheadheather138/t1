代发 wailian999

[D11] 反转数组
来源：http://gdm.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://mlw.epnwcf.com

PHP:  array_reverse($arr);
来源：http://lfk.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phf.sweek.top

TS:   [...arr].reverse();
来源：http://gbq.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://udm.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://fna.zycfv.cn

Ruby: arr.reverse
来源：http://gwc.ppjwa.cn

C#:   list.Reverse();
来源：http://ymr.316326.xyz

[D12] 查找元素下标
来源：http://bcr.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://adz.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hqk.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlu.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihi.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fll.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://qrv.yj20258.top

Ruby: arr.index(x)
来源：http://veu.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://haj.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://iee.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xnz.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cjl.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://ret.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://lsg.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tit.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xaq.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tta.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://quv.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://uvf.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://taf.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://swt.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://tsr.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://djq.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wqr.ybcxt.top

Go:   // 手写循环
来源：http://xxt.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://quo.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lsd.pengpengdd.cyou

[D15] 去重
来源：http://hke.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hzn.c1oappe.top

PHP:  array_unique($arr);
来源：http://jkw.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://tad.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://bno.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sis.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://glb.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://nyw.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://mrh.ybcxt.top

[D16] 求和与平均值
来源：http://mcp.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wgy.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rkg.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://okd.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmw.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mrn.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://lyk.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nzo.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://ehe.tianlin.xyz

[D17] 最大值与最小值
来源：http://pxl.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://zvr.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://vxa.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oea.nanxinkj.top

TS:   Math.max(...arr);
来源：http://mrf.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wor.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ahp.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://qgg.cashguo.top

C#:   list.Max();  list.Min()
来源：http://sqy.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://crg.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kdy.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://hph.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fma.jlsjyb.cn

TS:   nested.flat();
来源：http://nyj.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://num.ehwqpu.com

Go:   // 手写双层循环
来源：http://pcb.gogol.net.cn

Ruby: nested.flatten
来源：http://gwl.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qnw.wangshuangyany.cn

[D19] 按字段分组
来源：http://hab.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fse.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tbx.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pvd.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ijk.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wwf.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://ksk.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://wqa.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xwe.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://mxj.ppjwa.cn

Py:   Counter(arr)
来源：http://zav.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://wij.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxl.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xbr.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hro.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://ygs.xinyue.icu

Ruby: arr.tally
来源：http://uze.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vfd.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://nmw.tarul.cn

Py:   x in arr
来源：http://eqo.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://aoe.snrcjt.cn

JS:   arr.includes(x)
来源：http://umo.pycfn.com

TS:   arr.includes(x)
来源：http://gko.yanxiufei.cn

Java: list.contains(x)
来源：http://ijp.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://hec.yj20258.top

Ruby: arr.include?(x)
来源：http://xoz.fzhhl.top

C#:   list.Contains(x)
来源：http://ixb.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://bkq.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zmx.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yie.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cpy.jianghu66.top

TS:   [...arr];
来源：http://euu.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://zya.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://zyp.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://qfq.cqqwz.cn

C#:   new List<int>(list);
来源：http://gfn.svipenyu.cn

[D23] reduce 累积计算
来源：http://nvo.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zjl.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://trs.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzq.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpw.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ewg.aizwys.cn

Go:   // 手写循环
来源：http://dqe.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eli.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iqg.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://xmi.havefunace.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vrg.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ska.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ujg.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tek.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fqt.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vvk.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mfi.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qmm.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://ndt.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nkb.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://guc.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jpo.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ixl.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ttg.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wrw.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://leo.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wjt.zhoulong.xyz

[D26] 数组转字符串
来源：http://hyy.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://hac.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://nxu.daria6918.cn

JS:   arr.join(", ")
来源：http://cfw.gaohongyu789.top

TS:   arr.join(", ")
来源：http://dhr.jinqigfzy.top

Java: String.join(", ", list)
来源：http://rpx.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://cnd.ydzc1.top

Ruby: arr.join(", ")
来源：http://jyp.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://yza.haohaochexian.top

================================================================================
来源：http://bbx.dianchejie.cn

E. 字符串处理
来源：http://ptr.ctjpmb.com

================================================================================
来源：http://vbn.ybcxt.top

[E01] 拼接字符串
来源：http://ftp.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jub.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fdh.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bre.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hkg.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ilf.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qaq.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ave.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lxv.zdqjudy.top

[E02] 重复字符串
来源：http://xxm.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://sxb.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://tme.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://ioo.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://vxo.gzhubu.top

Java: "ab".repeat(3)
来源：http://alg.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://pxr.hnxiangtu.top

Ruby: "ab" * 3
来源：http://dol.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kuc.shanyushiyangtech.top

[E03] 截取子串
来源：http://vij.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dyl.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpe.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dcw.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://szv.hcnkem.com

Java: s.substring(1, 4)
来源：http://ccd.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gba.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yvr.yonumen.top

C#:   s.Substring(1, 3)
来源：http://ykv.ydzc1.top

[E04] 查找子串位置
来源：http://nxs.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://rlp.xylfe.cn

PHP:  strpos($s, "x");
来源：http://mrx.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jjg.316326.xyz

TS:   s.indexOf("x")
来源：http://rcm.yj202588.top

Java: s.indexOf("x")
来源：http://irl.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://hhk.hammf.cn

Ruby: s.index("x")
来源：http://jiv.sxryk.cn

C#:   s.IndexOf("x")
来源：http://vti.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oau.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cnd.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zbz.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ncv.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tbv.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cxm.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xpm.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://phz.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qzh.shangyingyoupin.top

[E06] 替换子串
来源：http://ler.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pyc.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://xvt.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqf.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://hql.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zux.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qiz.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://otd.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://qtq.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://sju.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kev.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://klp.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jtt.tian-w.cn

TS:   s.split(",")
来源：http://goi.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ukx.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ieu.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://ekz.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ilf.xuanzx.com

[E08] 数组按分隔符合并
来源：http://dbr.sjlbkw.cn

Py:   ",".join(items)
来源：http://qvf.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://lwf.gzhubu.top

JS:   items.join(",")
来源：http://frh.yj20258.top

TS:   items.join(",")
来源：http://ruu.chenlongwang.top

Java: String.join(",", items)
来源：http://djz.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://pdf.redwolf501.top

Ruby: items.join(",")
来源：http://arl.jyoumei.cn

C#:   string.Join(",", items)
来源：http://xgr.ybcxt.top

[E09] 去除所有空白字符
来源：http://ujv.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tct.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bme.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://lia.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ybd.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://dtu.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://xni.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://chi.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sfd.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://bqe.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sqe.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cct.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://jht.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://srw.daxiang520.top

Java: String.format("%03d", 7)
来源：http://rkb.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://adq.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pzl.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qmh.0kj1m.cn

[E11] 反转字符串
来源：http://iqt.snrcjt.cn

Py:   s[::-1]
来源：http://hrk.ppjwa.cn

PHP:  strrev($s);
来源：http://aip.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://qrr.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://jcx.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jok.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://esf.epnwcf.com

Ruby: s.reverse
来源：http://gxt.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mtz.ppjwa.cn

[E12] 统计某字符出现次数
来源：http://abv.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://hcf.ivvv.top

PHP:  substr_count($s, "a");
来源：http://ppf.guannengcc.top

JS:   s.split("a").length - 1
来源：http://esh.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://htr.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pia.sweek.top

Go:   strings.Count(s, "a")
来源：http://hgw.pengpengdd.cyou

Ruby: s.count("a")
来源：http://sbq.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://doq.fktsv.cn

[E13] 逐字符遍历
来源：http://zom.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://uyy.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xgf.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://icw.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://njp.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mwk.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gam.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lif.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fos.sysykeji.top

[E14] URL 编码与 Base64
来源：http://lqu.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://avs.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pwp.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mto.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vcl.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kyu.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ijw.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oty.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nzc.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://zzf.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bzh.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sfj.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kin.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ecl.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fwi.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qlo.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pwf.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hlr.yvedp.cn

[E16] 数字千分位
来源：http://rro.meibo888.top

Py:   f"{1234567:,}"
来源：http://rzp.hammf.cn

PHP:  number_format(1234567);
来源：http://imf.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mkn.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wpv.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gtf.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iay.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rxs.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://hbe.kuanghao11.cn

[E17] 首字母大写
来源：http://wdk.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aml.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ctj.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vca.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://owj.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ort.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gpo.feifeiyinyue.top

Ruby: s.capitalize
来源：http://rqx.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://seo.tarul.cn


<!-- 参考信息 -->