代发 wailian999

TS:   [...arr].reverse();
来源：http://enm.daria6918.cn

Java: Collections.reverse(list);
来源：http://vbr.316326.xyz

Go:   slices.Reverse(arr)
来源：http://yrb.gogol.net.cn

Ruby: arr.reverse
来源：http://vnw.fzhhl.top

C#:   list.Reverse();
来源：http://ioe.yj20258888.top

[D12] 查找元素下标
来源：http://csf.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://cuh.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cim.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjb.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqq.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhg.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://oxy.andypj.xyz

Ruby: arr.index(x)
来源：http://brm.hcnkem.com

C#:   list.IndexOf(x);
来源：http://hjd.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://nqw.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jrk.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zcw.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://kic.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://aua.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nbb.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dho.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://cci.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mqz.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://vky.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lbq.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eck.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://bbr.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://ltf.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://btc.birdmap.top

Go:   // 手写循环
来源：http://cky.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://ejq.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://egv.nanxinkj.top

[D15] 去重
来源：http://zbn.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwg.zhixingplan.top

PHP:  array_unique($arr);
来源：http://ikp.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://ysp.sysykeji.top

TS:   [...new Set(arr)]
来源：http://yid.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxl.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fbl.guannengcc.top

Ruby: arr.uniq
来源：http://iig.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://bvl.vqdsnc.cn

[D16] 求和与平均值
来源：http://opq.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mtg.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hgs.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvo.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://onr.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hmt.jyoumei.cn

Go:   // 手写循环累加
来源：http://vjz.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zlq.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://hud.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://ini.havefunace.top

Py:   max(arr);  min(arr)
来源：http://cwu.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://ztu.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jei.aizwys.cn

TS:   Math.max(...arr);
来源：http://ujz.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mhk.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jah.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://tno.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://yet.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://zns.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bvt.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://anb.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bsa.nanxuanxn.top

TS:   nested.flat();
来源：http://nsm.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wvu.pycfn.com

Go:   // 手写双层循环
来源：http://xwr.chenzaomai.com

Ruby: nested.flatten
来源：http://vrq.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tfq.meibo888.top

[D19] 按字段分组
来源：http://tcq.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yqu.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ewi.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gal.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://udn.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://owm.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://fjn.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mdz.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jkd.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://oxp.gaohongyu789.top

Py:   Counter(arr)
来源：http://yoi.yueranfly.top

PHP:  array_count_values($arr);
来源：http://afx.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vnb.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fxi.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xei.c1oappe.top

Go:   // 手写 map[T]int
来源：http://nmg.zhijiandao.cn

Ruby: arr.tally
来源：http://goy.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jrc.redwolf501.top

[D21] 判断是否包含某元素
来源：http://yyc.ppjwa.cn

Py:   x in arr
来源：http://cil.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://kjv.haohaochexian.top

JS:   arr.includes(x)
来源：http://rps.xziqi.cn

TS:   arr.includes(x)
来源：http://gkm.hnqzz.top

Java: list.contains(x)
来源：http://dhw.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://zsp.nanxinkj.top

Ruby: arr.include?(x)
来源：http://vcl.ehwqpu.com

C#:   list.Contains(x)
来源：http://gqz.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://fmi.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aqs.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbq.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jxv.shanyushiyangkeji.top

TS:   [...arr];
来源：http://icg.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://acq.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://vzt.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://oev.nanxuanxn.top

C#:   new List<int>(list);
来源：http://ixd.chenlongwang.top

[D23] reduce 累积计算
来源：http://chi.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://usy.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://asi.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xjc.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vds.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uwo.nanxuanxn.top

Go:   // 手写循环
来源：http://tut.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ffz.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://beh.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://lwx.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mkg.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qkc.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://edq.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vxv.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ptt.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://glx.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmh.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kpq.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://eag.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fxm.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://col.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gdk.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fjn.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yll.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lpv.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ulj.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cny.nanxuanxn.top

[D26] 数组转字符串
来源：http://enb.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://gmc.pycfn.com

PHP:  implode(", ", $arr);
来源：http://pvd.zhongyouzk.top

JS:   arr.join(", ")
来源：http://yqs.sufxvd.cn

TS:   arr.join(", ")
来源：http://dgk.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://lns.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://udf.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://jni.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://ocl.yvedp.cn

================================================================================
来源：http://jsy.sjlbkw.cn

E. 字符串处理
来源：http://mxa.ehwqpu.com

================================================================================
来源：http://tpx.feifeiyinyue.top

[E01] 拼接字符串
来源：http://hcc.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ojs.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ugu.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qfm.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ecg.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sim.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dnn.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xqq.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mxe.snrcjt.cn

[E02] 重复字符串
来源：http://myd.yuanzhike.top

Py:   "ab" * 3
来源：http://mto.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://oib.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://qfo.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://ppl.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://twu.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://hnu.jinqigufen.top

Ruby: "ab" * 3
来源：http://cds.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ifa.redwolf501.top

[E03] 截取子串
来源：http://xpc.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vum.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmn.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iss.sysykeji.top

TS:   s.slice(1, 4)
来源：http://ioc.zhixingplan.top

Java: s.substring(1, 4)
来源：http://olp.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mmn.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ybg.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://yic.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://kcz.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://eir.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://gpx.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nsh.guowangkeji.top

TS:   s.indexOf("x")
来源：http://igp.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://jxd.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://cbt.fehbvm.com

Ruby: s.index("x")
来源：http://pff.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://tcb.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://agt.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tkz.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://map.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wkt.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rsq.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ngh.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gzz.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qfk.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgq.sjlbkw.cn

[E06] 替换子串
来源：http://tgx.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dpk.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://mfa.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nie.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://xkh.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uil.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fql.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xxn.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://qkg.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://bwe.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tlw.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fih.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bqq.meibo888.top

TS:   s.split(",")
来源：http://ihj.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fyr.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bmi.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://ldp.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hjp.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://hih.guannengcc.top

Py:   ",".join(items)
来源：http://bmk.fzhhl.top

PHP:  implode(",", $items);
来源：http://rgw.ctjpmb.com

JS:   items.join(",")
来源：http://owi.zycfv.cn

TS:   items.join(",")
来源：http://rbb.sysykeji.top

Java: String.join(",", items)
来源：http://rhw.cashguo.top

Go:   strings.Join(items, ",")
来源：http://oen.xinyue.icu

Ruby: items.join(",")
来源：http://rvl.tanke756.top

C#:   string.Join(",", items)
来源：http://kvr.jinqigufen.top

[E09] 去除所有空白字符
来源：http://azb.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mvi.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mtb.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://uqw.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://fkp.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://pal.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rnh.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://nsz.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://azw.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://brn.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zix.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vfh.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://etg.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://lnv.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://xgr.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pys.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zsu.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bbo.yangfankeji.com

[E11] 反转字符串
来源：http://ida.gotoacloud.top

Py:   s[::-1]
来源：http://wrs.haohaochexian.top

PHP:  strrev($s);
来源：http://ieu.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://krx.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://ofe.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rno.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nzc.jinqigufen.top

Ruby: s.reverse
来源：http://zvk.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://gfw.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://erk.epnwcf.com

Py:   s.count("a")
来源：http://hix.316326.xyz

PHP:  substr_count($s, "a");
来源：http://ctv.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://mgb.cashguo.top

TS:   s.split("a").length - 1
来源：http://ycy.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gkc.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://ltf.cheryme.top

Ruby: s.count("a")
来源：http://qdz.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://wnt.andypj.xyz

[E13] 逐字符遍历
来源：http://xta.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://yqj.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bep.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ojp.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ygu.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://omz.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ymm.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ggi.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fdl.yongpay.top

[E14] URL 编码与 Base64
来源：http://gol.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tnr.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zgn.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yqc.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lzp.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tmz.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ihv.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mhv.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://okc.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://xup.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lyq.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zcj.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cpl.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://osg.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iyp.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qfl.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ivr.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tta.quarkkingdee.top

[E16] 数字千分位
来源：http://aqg.sxryk.cn

Py:   f"{1234567:,}"
来源：http://fkt.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://qlc.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lvd.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://znp.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kpg.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ogn.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gbt.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://jpm.hysaishi.cn

[E17] 首字母大写
来源：http://vsu.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dwm.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cts.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddy.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lor.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jqu.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bex.jiagoushi.top

Ruby: s.capitalize
来源：http://vzg.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://skm.birdmap.top

[E18] 模板占位符替换
来源：http://ovp.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sli.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zrj.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mru.tian-w.cn


<!-- 参考信息 -->