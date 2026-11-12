代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsp.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmx.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wss.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://qyb.svipenyu.cn

Ruby: arr.index(x)
来源：http://jqz.ybcxt.top

C#:   list.IndexOf(x);
来源：http://ubw.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://umn.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mod.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jnl.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://rds.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://qwm.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gmi.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zom.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://air.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pwu.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://hwn.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rvk.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fes.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://kmi.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://hbv.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zdu.meibo888.top

Go:   // 手写循环
来源：http://pfk.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://eth.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vew.52xcode.cn

[D15] 去重
来源：http://vhp.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ugo.cheryme.top

PHP:  array_unique($arr);
来源：http://fbk.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://wrj.uphjek.com

TS:   [...new Set(arr)]
来源：http://pty.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pae.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sad.shuidangran.top

Ruby: arr.uniq
来源：http://slg.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://awt.shzxlz.cn

[D16] 求和与平均值
来源：http://sdr.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xdk.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nfo.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xag.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ngf.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nke.daxiang520.top

Go:   // 手写循环累加
来源：http://pdb.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vfr.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://nju.xylfe.cn

[D17] 最大值与最小值
来源：http://uap.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://waz.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://ocz.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rpi.fzhhl.top

TS:   Math.max(...arr);
来源：http://dvq.chenjidiqi.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://zdl.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fkp.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://qng.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://zwz.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://epe.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xwc.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mfj.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sxy.epnwcf.com

TS:   nested.flat();
来源：http://oek.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lfo.bbcook.cn

Go:   // 手写双层循环
来源：http://zwx.0kj1m.cn

Ruby: nested.flatten
来源：http://ivx.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bvj.pycfn.com

[D19] 按字段分组
来源：http://rfc.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqs.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kpp.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dzy.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wvu.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ori.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://uwp.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://izp.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yhn.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://ngw.gogol.net.cn

Py:   Counter(arr)
来源：http://igw.sysykeji.top

PHP:  array_count_values($arr);
来源：http://noj.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhf.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fhs.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qnt.316326.xyz

Go:   // 手写 map[T]int
来源：http://lyi.mhx1999.top

Ruby: arr.tally
来源：http://uzg.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rtg.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://euv.sufxvd.cn

Py:   x in arr
来源：http://qng.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://dqt.svipenyu.cn

JS:   arr.includes(x)
来源：http://tcy.hysaishi.cn

TS:   arr.includes(x)
来源：http://xlw.cqqwz.cn

Java: list.contains(x)
来源：http://hxs.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://csk.epnwcf.com

Ruby: arr.include?(x)
来源：http://xpz.jqgufenzy.top

C#:   list.Contains(x)
来源：http://ohb.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://hkd.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://udp.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abu.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mjm.xylfe.cn

TS:   [...arr];
来源：http://unc.sysykeji.top

Java: new ArrayList<>(list);
来源：http://les.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wej.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://jbv.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://wym.jyoumei.cn

[D23] reduce 累积计算
来源：http://jhg.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jlq.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yqg.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqj.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glp.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xxn.gotoacloud.top

Go:   // 手写循环
来源：http://kew.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xnh.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dkf.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://khj.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mhw.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mec.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vur.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gmq.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jzx.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bis.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rvq.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eqc.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://llo.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jof.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdu.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qoa.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://afx.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zss.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vfs.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vtk.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zyf.gzhubu.top

[D26] 数组转字符串
来源：http://psn.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://mmv.cheryme.top

PHP:  implode(", ", $arr);
来源：http://pex.jiagoushi.top

JS:   arr.join(", ")
来源：http://otb.ctjpmb.com

TS:   arr.join(", ")
来源：http://tcv.smart0.xyz

Java: String.join(", ", list)
来源：http://iml.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://kux.yonumen.top

Ruby: arr.join(", ")
来源：http://rir.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://ruj.gotoacloud.top

================================================================================
来源：http://qyj.snrcjt.cn

E. 字符串处理
来源：http://voj.tian-w.cn

================================================================================
来源：http://npw.zhongyouzk.top

[E01] 拼接字符串
来源：http://plu.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyn.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcf.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zmj.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvv.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://phh.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://moa.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rkg.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://shx.xinyue.icu

[E02] 重复字符串
来源：http://nkc.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://agy.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://jdh.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://shl.hcnkem.com

TS:   "ab".repeat(3)
来源：http://hrh.chenzaomai.com

Java: "ab".repeat(3)
来源：http://ivt.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://mvt.tarul.cn

Ruby: "ab" * 3
来源：http://dnn.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://abx.yanxiufei.cn

[E03] 截取子串
来源：http://hsl.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lpu.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zxu.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://njd.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://mhm.xziqi.cn

Java: s.substring(1, 4)
来源：http://rrz.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://izq.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bah.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://wbb.jyoumei.cn

[E04] 查找子串位置
来源：http://beq.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://fsp.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://vlw.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qqo.xziqi.cn

TS:   s.indexOf("x")
来源：http://vnt.havefunace.top

Java: s.indexOf("x")
来源：http://mxd.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://hru.zhixingplan.top

Ruby: s.index("x")
来源：http://axb.tanke756.top

C#:   s.IndexOf("x")
来源：http://iqs.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://oel.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cwj.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qxc.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bjt.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fwg.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qjd.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ssw.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cwk.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rsb.sjlbkw.cn

[E06] 替换子串
来源：http://ukn.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kmw.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://xmq.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwr.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://brw.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vzm.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zzm.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bes.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://imu.ybcxt.top

[E07] 按分隔符拆分
来源：http://ykh.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://piy.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eco.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rly.sjlbkw.cn

TS:   s.split(",")
来源：http://vkj.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://hwx.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pev.pycfn.com

Ruby: s.split(",");  s.split
来源：http://vtl.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pbg.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://oez.pengpengdd.cyou

Py:   ",".join(items)
来源：http://pqq.0kj1m.cn

PHP:  implode(",", $items);
来源：http://njx.hammf.cn

JS:   items.join(",")
来源：http://xbs.cdnleiting.top

TS:   items.join(",")
来源：http://dqq.hfpthk.cn

Java: String.join(",", items)
来源：http://rtg.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://jkw.fktsv.cn

Ruby: items.join(",")
来源：http://adc.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://wha.ybcxt.top

[E09] 去除所有空白字符
来源：http://eei.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ejf.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dgo.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://clq.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://gzo.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://egt.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tye.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://qvh.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kcd.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://onn.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bxh.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ays.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://vdj.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://hmz.fzhhl.top

Java: String.format("%03d", 7)
来源：http://ewi.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hzu.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kmm.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sek.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://okm.yj202588.top

Py:   s[::-1]
来源：http://ntq.zhoulong.xyz

PHP:  strrev($s);
来源：http://oks.tanke756.top

JS:   [...s].reverse().join("")
来源：http://cmy.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://zaw.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jwe.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sgq.chenlongwang.top

Ruby: s.reverse
来源：http://lxz.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://yoz.hammf.cn

[E12] 统计某字符出现次数
来源：http://utf.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://bdg.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://oia.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://mny.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://pvq.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://idn.tanke756.top

Go:   strings.Count(s, "a")
来源：http://hyd.dianchejie.cn

Ruby: s.count("a")
来源：http://pzq.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://uby.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://ecs.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://vgp.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bev.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xja.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qqq.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://biu.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gqw.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vrt.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gft.zycfv.cn

[E14] URL 编码与 Base64
来源：http://guz.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fvh.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hoi.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://stl.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fpn.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cmh.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qvl.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yup.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hmy.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://nbd.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wyn.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://swp.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bfj.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cqi.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uop.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blw.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oyk.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyc.316326.xyz

[E16] 数字千分位
来源：http://ykm.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://xes.nwbrower.top

PHP:  number_format(1234567);
来源：http://jsz.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ogc.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qhx.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dwk.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cqe.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cdf.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://yod.cashguo.top

[E17] 首字母大写
来源：http://emx.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ixr.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rgj.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jdu.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqo.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ajq.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://acc.chenlongwang.top

Ruby: s.capitalize
来源：http://hrw.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rlo.quarkkingdee.top

[E18] 模板占位符替换
来源：http://rus.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vll.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ftb.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mfw.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://mkj.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jyl.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vqk.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dpu.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bza.yj20258888.top

[E19] 多行文本按行拆分
来源：http://hjv.c1oappe.top

Py:   s.splitlines()
来源：http://dvg.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nut.mhx1999.top


<!-- 参考信息 -->