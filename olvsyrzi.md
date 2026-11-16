代发 wailian999

C#:   list.Reverse();
来源：http://gxx.daria6918.cn

[D12] 查找元素下标
来源：http://ksu.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://dvc.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://clt.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tiy.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjq.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qxk.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://fmb.zhongyouzk.top

Ruby: arr.index(x)
来源：http://tno.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://vkx.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://nij.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gbb.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nbo.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://zbf.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://hux.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hje.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wzh.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kcy.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://adm.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://gjv.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yvj.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vem.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://tae.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://pdm.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nxn.vqdsnc.cn

Go:   // 手写循环
来源：http://ift.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://yde.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://kkh.jyoumei.cn

[D15] 去重
来源：http://axx.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xgu.jinqigufen.top

PHP:  array_unique($arr);
来源：http://dpt.nwbrower.top

JS:   [...new Set(arr)]
来源：http://par.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://oyb.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://php.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://faw.bjfxy.top

Ruby: arr.uniq
来源：http://itv.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://ver.tarul.cn

[D16] 求和与平均值
来源：http://gpg.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ypc.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zwn.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dwr.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jdu.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lqy.dashuyun.cn

Go:   // 手写循环累加
来源：http://edg.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://noz.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://uab.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://uge.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://tkq.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://xzt.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pju.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://ewo.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mqr.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqf.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://sgv.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://jsq.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://kes.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vpa.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://xwi.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://arm.xuanzx.com

TS:   nested.flat();
来源：http://lds.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nkw.xuanzx.com

Go:   // 手写双层循环
来源：http://ykz.pengpengdd.cyou

Ruby: nested.flatten
来源：http://ucy.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://txe.sufxvd.cn

[D19] 按字段分组
来源：http://ses.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oow.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iiq.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxu.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gff.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lrn.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://eed.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vwk.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://sji.jiagoushi.top

Py:   Counter(arr)
来源：http://pct.sweek.top

PHP:  array_count_values($arr);
来源：http://wwm.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhx.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ery.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ztz.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://dzr.epnwcf.com

Ruby: arr.tally
来源：http://mmr.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oom.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://gyn.zdqjudy.top

Py:   x in arr
来源：http://vyg.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://umv.cheryme.top

JS:   arr.includes(x)
来源：http://gdz.jlsjyb.cn

TS:   arr.includes(x)
来源：http://pgs.shanyushiyangtech.top

Java: list.contains(x)
来源：http://apb.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://ehj.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://dgd.havefunace.top

C#:   list.Contains(x)
来源：http://tcw.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://ohm.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pkf.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gvi.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://acg.epnwcf.com

TS:   [...arr];
来源：http://qbj.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://jzb.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://ned.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://twh.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://jpz.meibo888.top

[D23] reduce 累积计算
来源：http://ced.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kke.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qux.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uiv.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlk.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tnz.cucudq.cn

Go:   // 手写循环
来源：http://oia.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ylr.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oaj.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://oag.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yod.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nic.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pez.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zwm.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xif.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgh.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iis.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kbh.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://iqm.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rty.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://prh.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvj.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rni.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sur.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mij.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://odh.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zii.tarul.cn

[D26] 数组转字符串
来源：http://gtw.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://dzh.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://uyl.smart0.xyz

JS:   arr.join(", ")
来源：http://fet.yuxming.cn

TS:   arr.join(", ")
来源：http://gka.ybcxt.top

Java: String.join(", ", list)
来源：http://ojw.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://blr.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://dvl.tanke756.top

C#:   string.Join(", ", list)
来源：http://xdx.shuidangran.top

================================================================================
来源：http://obc.zycfv.cn

E. 字符串处理
来源：http://zyu.hysaishi.cn

================================================================================
来源：http://ztl.bbcook.cn

[E01] 拼接字符串
来源：http://mnq.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gww.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ixp.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://svi.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vld.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nlj.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gey.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tph.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tnz.zhixingplan.top

[E02] 重复字符串
来源：http://ceh.tian-w.cn

Py:   "ab" * 3
来源：http://egn.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://wfm.yuxming.cn

JS:   "ab".repeat(3)
来源：http://kra.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://bsx.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://jfl.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://fyx.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://bmp.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qkw.ivvv.top

[E03] 截取子串
来源：http://mtm.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jcv.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kwe.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uwk.hnqzz.top

TS:   s.slice(1, 4)
来源：http://ciu.9152youxi.cn

Java: s.substring(1, 4)
来源：http://nee.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uas.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://ulx.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://kvw.zhixingplan.top

[E04] 查找子串位置
来源：http://cjx.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://ayq.tian-w.cn

PHP:  strpos($s, "x");
来源：http://vdm.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ozv.tarul.cn

TS:   s.indexOf("x")
来源：http://rks.gotoacloud.top

Java: s.indexOf("x")
来源：http://cje.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://fmk.sufxvd.cn

Ruby: s.index("x")
来源：http://zam.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://pff.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wex.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wdq.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nvl.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gcq.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qkc.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfk.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezn.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvw.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cyx.xylfe.cn

[E06] 替换子串
来源：http://zek.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pxu.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://pwh.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqv.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://lvb.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpw.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qwd.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dui.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://qag.daxiang520.top

[E07] 按分隔符拆分
来源：http://vij.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uvh.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oij.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://quy.dianchejie.cn

TS:   s.split(",")
来源：http://vla.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://aqn.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wyl.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://tri.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://guw.xinyue.icu

[E08] 数组按分隔符合并
来源：http://hrq.cashguo.top

Py:   ",".join(items)
来源：http://xfp.yvedp.cn

PHP:  implode(",", $items);
来源：http://gfm.shuidangran.top

JS:   items.join(",")
来源：http://qgk.shanyushiyangtech.top

TS:   items.join(",")
来源：http://tak.sxryk.cn

Java: String.join(",", items)
来源：http://ouq.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://cvw.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://rvr.dianchejie.cn

C#:   string.Join(",", items)
来源：http://yhl.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://igv.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qxv.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jfr.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://fuz.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://ncn.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://aqw.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rxk.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://elq.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mpf.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://awv.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gld.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kxf.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://dwp.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://upp.yj202588.top

Java: String.format("%03d", 7)
来源：http://opv.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://uhu.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ytq.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://akd.hesvh.cn

[E11] 反转字符串
来源：http://ahw.yvedp.cn

Py:   s[::-1]
来源：http://skx.yj20258.top

PHP:  strrev($s);
来源：http://wym.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://pim.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://rzc.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dzn.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ivi.wangshuangyany.cn

Ruby: s.reverse
来源：http://lkz.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://yfh.fengsongda.top

[E12] 统计某字符出现次数
来源：http://qge.pengpengdd.cyou

Py:   s.count("a")
来源：http://ypi.yj202588.top

PHP:  substr_count($s, "a");
来源：http://ihy.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://jkv.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://kov.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ctk.birdmap.top

Go:   strings.Count(s, "a")
来源：http://wcq.xuanzx.com

Ruby: s.count("a")
来源：http://qwt.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://tqa.gotoacloud.top

[E13] 逐字符遍历
来源：http://sdp.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://oys.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://soi.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sos.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xqy.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pnt.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qpx.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bds.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fqu.vehdjk.com

[E14] URL 编码与 Base64
来源：http://pyg.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://set.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xfr.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://elf.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aht.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xot.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iok.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fbr.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spw.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://kzw.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fwd.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ibr.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://avr.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nhy.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cwt.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yyg.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xir.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dpv.pengpengdd.cyou

[E16] 数字千分位
来源：http://zsm.andypj.xyz

Py:   f"{1234567:,}"
来源：http://frx.dianchejie.cn

PHP:  number_format(1234567);
来源：http://afb.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://cvu.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://awa.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jsc.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ujn.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kxu.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://hbp.52xcode.cn

[E17] 首字母大写
来源：http://dju.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zxe.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hbu.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mog.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iyr.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ijp.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dzl.zdbjq.cn

Ruby: s.capitalize
来源：http://pin.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ezn.bbcook.cn

[E18] 模板占位符替换
来源：http://jhr.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tsj.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfc.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iyf.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://sgl.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://awb.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://irp.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fnn.redwolf501.top


<!-- 参考信息 -->