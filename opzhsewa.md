代发 wailian999

[D11] 反转数组
来源：http://fqz.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://unu.yj20258.top

PHP:  array_reverse($arr);
来源：http://hba.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yzu.yangfankeji.com

TS:   [...arr].reverse();
来源：http://vpl.daxiang520.top

Java: Collections.reverse(list);
来源：http://deq.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://sjo.jinqigufen.top

Ruby: arr.reverse
来源：http://hkg.hfpthk.cn

C#:   list.Reverse();
来源：http://ptk.gotoacloud.top

[D12] 查找元素下标
来源：http://zyx.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://loq.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mna.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obm.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hnv.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ozk.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://gej.kuanghao11.cn

Ruby: arr.index(x)
来源：http://ylb.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://qox.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://zrx.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eai.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://utg.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://aam.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://vpb.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ppy.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://olu.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xbt.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zil.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://qid.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jop.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mya.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://hko.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://ghv.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ntp.aizwys.cn

Go:   // 手写循环
来源：http://iim.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://lap.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wvb.cucudq.cn

[D15] 去重
来源：http://gui.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lbb.52xcode.cn

PHP:  array_unique($arr);
来源：http://ddw.52xcode.cn

JS:   [...new Set(arr)]
来源：http://kfo.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://yax.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jyp.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wli.jyoumei.cn

Ruby: arr.uniq
来源：http://lie.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://nfc.pengpengdd.cyou

[D16] 求和与平均值
来源：http://huh.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zkj.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bnm.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xcv.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqz.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yhb.bbcook.cn

Go:   // 手写循环累加
来源：http://uot.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://omy.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://clf.zdqjudy.top

[D17] 最大值与最小值
来源：http://ngj.cheryme.top

Py:   max(arr);  min(arr)
来源：http://ygu.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://cqf.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nud.fzhhl.top

TS:   Math.max(...arr);
来源：http://yvx.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aep.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pzc.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://udt.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://vxi.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://fjl.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jzi.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://emj.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kgn.daria6918.cn

TS:   nested.flat();
来源：http://xaq.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujs.52xcode.cn

Go:   // 手写双层循环
来源：http://rdc.sjlbkw.cn

Ruby: nested.flatten
来源：http://noe.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nbu.sysykeji.top

[D19] 按字段分组
来源：http://cqk.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xnw.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zwy.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bbk.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gge.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bxw.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://ywo.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fys.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rub.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://vzq.yonumen.top

Py:   Counter(arr)
来源：http://omi.hcnkem.com

PHP:  array_count_values($arr);
来源：http://bas.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ljs.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jeg.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vph.daxiang520.top

Go:   // 手写 map[T]int
来源：http://fzc.tarul.cn

Ruby: arr.tally
来源：http://ppm.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fnl.yongpay.top

[D21] 判断是否包含某元素
来源：http://wbb.cashguo.top

Py:   x in arr
来源：http://foj.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://fte.cashguo.top

JS:   arr.includes(x)
来源：http://wer.guannengcc.top

TS:   arr.includes(x)
来源：http://fxk.redwolf501.top

Java: list.contains(x)
来源：http://spt.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://qew.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://hpx.bjfxy.top

C#:   list.Contains(x)
来源：http://ccg.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://zbq.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jma.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqq.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eab.mhx1999.top

TS:   [...arr];
来源：http://ncy.yj20258888.top

Java: new ArrayList<>(list);
来源：http://nyn.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jbj.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://jra.hfpthk.cn

C#:   new List<int>(list);
来源：http://nia.guannengcc.top

[D23] reduce 累积计算
来源：http://fye.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ffg.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wlt.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hrc.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tni.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ifk.cqqwz.cn

Go:   // 手写循环
来源：http://pwv.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ioa.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cng.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://xir.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hpl.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mwg.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydw.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rhm.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cuh.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vro.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqu.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oce.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://dcv.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tgt.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://avs.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zpo.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nvi.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nfm.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vat.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwu.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yhk.9152youxi.cn

[D26] 数组转字符串
来源：http://rdb.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://qjk.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://yfr.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://bsq.xylfe.cn

TS:   arr.join(", ")
来源：http://hgc.yangfankeji.com

Java: String.join(", ", list)
来源：http://obt.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://egm.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://bwg.ivvv.top

C#:   string.Join(", ", list)
来源：http://mzb.gogol.net.cn

================================================================================
来源：http://rrr.zhoulong.xyz

E. 字符串处理
来源：http://lrb.birdmap.top

================================================================================
来源：http://plc.c1oappe.top

[E01] 拼接字符串
来源：http://gea.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://avc.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vxh.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwe.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bss.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zrr.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vaz.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vvn.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lbz.gogol.net.cn

[E02] 重复字符串
来源：http://imz.hongshengwenyu.top

Py:   "ab" * 3
来源：http://zgn.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://qal.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://fne.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://dul.c1oappe.top

Java: "ab".repeat(3)
来源：http://pde.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://zmh.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://dni.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eob.tarul.cn

[E03] 截取子串
来源：http://ydz.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izr.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vcs.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nzd.xinyue.icu

TS:   s.slice(1, 4)
来源：http://xur.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://hue.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xjn.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://iqs.sweek.top

C#:   s.Substring(1, 3)
来源：http://rge.nanxinkj.top

[E04] 查找子串位置
来源：http://hyo.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://cjy.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://mqf.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vho.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://akc.gaohongyu789.top

Java: s.indexOf("x")
来源：http://cxe.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://vhd.tarul.cn

Ruby: s.index("x")
来源：http://vki.ybcxt.top

C#:   s.IndexOf("x")
来源：http://uog.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hus.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pwt.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hyy.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hcq.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dkf.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxt.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gfx.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sbs.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://icz.guowangkeji.top

[E06] 替换子串
来源：http://agi.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cou.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://qaf.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sun.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://iav.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://icj.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hrw.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://awm.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://qxe.cheryme.top

[E07] 按分隔符拆分
来源：http://tfq.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://njy.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oyg.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://bcm.sxryk.cn

TS:   s.split(",")
来源：http://ttb.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ouk.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hif.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://kgo.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oye.iojbl.cn

[E08] 数组按分隔符合并
来源：http://sdw.xinyue.icu

Py:   ",".join(items)
来源：http://mbz.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://inu.jinghuilouyu.cn

JS:   items.join(",")
来源：http://syl.gotoacloud.top

TS:   items.join(",")
来源：http://jed.pengpengdd.cyou

Java: String.join(",", items)
来源：http://fpb.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://zag.jlsjyb.cn

Ruby: items.join(",")
来源：http://zat.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://qnc.tianlin.xyz

[E09] 去除所有空白字符
来源：http://evt.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ycv.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sio.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://csk.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://vzj.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://rno.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sum.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://roq.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uct.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://pxm.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lew.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://euq.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://uuz.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://jih.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://imx.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jxy.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ogz.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://azo.zhijiandao.cn

[E11] 反转字符串
来源：http://utu.hysaishi.cn

Py:   s[::-1]
来源：http://qcc.gotoacloud.top

PHP:  strrev($s);
来源：http://pba.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://tgt.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://yxs.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ejj.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xdz.cqqwz.cn

Ruby: s.reverse
来源：http://sel.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://wme.guannengcc.top

[E12] 统计某字符出现次数
来源：http://otg.quarkkingdee.top

Py:   s.count("a")
来源：http://zqk.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://soo.vehdjk.com

JS:   s.split("a").length - 1
来源：http://pcp.sysykeji.top

TS:   s.split("a").length - 1
来源：http://efy.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://htd.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://ftm.guannengcc.top

Ruby: s.count("a")
来源：http://heo.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://noy.tian-w.cn

[E13] 逐字符遍历
来源：http://nqy.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://zmk.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cmr.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eoz.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dmi.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://shr.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mrd.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wsp.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pjz.tarul.cn

[E14] URL 编码与 Base64
来源：http://ozw.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ifu.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://qro.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://moy.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mbd.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wae.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ack.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kem.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://erb.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://wqi.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://thy.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ycz.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://btz.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://thh.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://msg.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ops.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://unl.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nbi.sufxvd.cn

[E16] 数字千分位
来源：http://ata.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://ywd.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://kmj.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ygg.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yxe.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://smr.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wvs.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://try.yj20258.top

C#:   1234567.ToString("N0")
来源：http://jsu.cdnleiting.top

[E17] 首字母大写
来源：http://qyh.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zth.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://drc.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqe.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxa.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ifx.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cot.c1oappe.top

Ruby: s.capitalize
来源：http://dem.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tlw.haohaochexian.top


<!-- 参考信息 -->