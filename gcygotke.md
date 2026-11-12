代发 wailian999

[D11] 反转数组
来源：http://slg.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://zne.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://tnq.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gsa.gogol.net.cn

TS:   [...arr].reverse();
来源：http://bau.xinyue.icu

Java: Collections.reverse(list);
来源：http://prc.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://hfm.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://zeq.kuanghao11.cn

C#:   list.Reverse();
来源：http://miv.jqgfzy.top

[D12] 查找元素下标
来源：http://mnl.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://qzc.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqy.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkh.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://adt.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phj.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://rsp.bbcook.cn

Ruby: arr.index(x)
来源：http://udd.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://kak.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://lzw.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qib.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hjs.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://ovj.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://buq.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qxv.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://epa.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://vig.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pug.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://ede.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imc.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kpr.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://raa.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://eby.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://czz.xziqi.cn

Go:   // 手写循环
来源：http://cry.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://boq.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vdp.gogol.net.cn

[D15] 去重
来源：http://ezj.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mcy.dashuyun.cn

PHP:  array_unique($arr);
来源：http://czv.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://edz.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://aqu.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://loz.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://ihp.tarul.cn

Ruby: arr.uniq
来源：http://pgq.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://cxy.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://pcm.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wex.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjw.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yqq.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nyh.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zhi.snrcjt.cn

Go:   // 手写循环累加
来源：http://jpj.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ruy.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://gle.andypj.xyz

[D17] 最大值与最小值
来源：http://jsp.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://rny.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://mim.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yiz.bbcook.cn

TS:   Math.max(...arr);
来源：http://aom.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://lle.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qfn.yongpay.top

Ruby: arr.max;  arr.min
来源：http://iic.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://jhn.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://rmn.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://peq.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://ntb.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://onu.birdmap.top

TS:   nested.flat();
来源：http://wug.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sbt.dashuyun.cn

Go:   // 手写双层循环
来源：http://joi.gzhubu.top

Ruby: nested.flatten
来源：http://kyz.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://avw.ehwqpu.com

[D19] 按字段分组
来源：http://uxw.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cps.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exv.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bxp.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pmk.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kxk.hammf.cn

Go:   // 手写 map[string][]T
来源：http://nmc.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://flw.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uyn.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://tie.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://oeh.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://nlj.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://san.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rst.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rvl.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://wmt.xylfe.cn

Ruby: arr.tally
来源：http://nhp.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hlj.ivvv.top

[D21] 判断是否包含某元素
来源：http://syy.ctjpmb.com

Py:   x in arr
来源：http://him.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://gsp.kuanghao11.cn

JS:   arr.includes(x)
来源：http://ieu.snrcjt.cn

TS:   arr.includes(x)
来源：http://jxc.jlsjyb.cn

Java: list.contains(x)
来源：http://bdz.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://vqb.daxiang520.top

Ruby: arr.include?(x)
来源：http://bsx.zhixingplan.top

C#:   list.Contains(x)
来源：http://bkr.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://uqa.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://otp.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cvf.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uty.yongpay.top

TS:   [...arr];
来源：http://uzs.hammf.cn

Java: new ArrayList<>(list);
来源：http://xyj.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lvp.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://swt.zdbjq.cn

C#:   new List<int>(list);
来源：http://kdc.ctjpmb.com

[D23] reduce 累积计算
来源：http://hdd.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyu.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vmn.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpy.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hbl.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://izv.feifeiyinyue.top

Go:   // 手写循环
来源：http://ktx.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qen.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pco.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://okr.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://krg.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ufy.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hjf.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qdc.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jsa.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wth.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbw.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mma.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://olc.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzp.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cou.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fzs.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wkd.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bad.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ihh.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://una.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jpf.kuanghao11.cn

[D26] 数组转字符串
来源：http://nkp.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://djp.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://lbx.dianchejie.cn

JS:   arr.join(", ")
来源：http://lsl.xylfe.cn

TS:   arr.join(", ")
来源：http://ktx.zhoulong.xyz

Java: String.join(", ", list)
来源：http://jnz.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://jtr.gotoacloud.top

Ruby: arr.join(", ")
来源：http://sfe.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://spr.fanxiaobao.xyz

================================================================================
来源：http://fii.sxryk.cn

E. 字符串处理
来源：http://tnb.gzhubu.top

================================================================================
来源：http://zdd.ppjwa.cn

[E01] 拼接字符串
来源：http://wlq.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gsp.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqe.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kfx.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ovm.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wat.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://axh.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tkh.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tmx.shanyushiyangtech.top

[E02] 重复字符串
来源：http://fvc.zhoulong.xyz

Py:   "ab" * 3
来源：http://vbm.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://vsd.redwolf501.top

JS:   "ab".repeat(3)
来源：http://fsr.xinyue.icu

TS:   "ab".repeat(3)
来源：http://aab.andypj.xyz

Java: "ab".repeat(3)
来源：http://nsp.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://tns.yj20258.top

Ruby: "ab" * 3
来源：http://zkd.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iiu.jqgufenzy.top

[E03] 截取子串
来源：http://hzc.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://abs.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://atz.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://edi.pycfn.com

TS:   s.slice(1, 4)
来源：http://cdz.bbcook.cn

Java: s.substring(1, 4)
来源：http://krf.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sok.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ysi.sweek.top

C#:   s.Substring(1, 3)
来源：http://qjr.dashuyun.cn

[E04] 查找子串位置
来源：http://hng.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://khv.bbcook.cn

PHP:  strpos($s, "x");
来源：http://yoi.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dhk.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://bpk.tarul.cn

Java: s.indexOf("x")
来源：http://avt.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://fjs.zdqjudy.top

Ruby: s.index("x")
来源：http://svk.c1oappe.top

C#:   s.IndexOf("x")
来源：http://slb.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fmc.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://erj.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hfp.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eaw.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dkf.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ddu.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vux.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oic.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wwg.svipenyu.cn

[E06] 替换子串
来源：http://fuw.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fcn.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ivi.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ziy.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://tfp.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vtd.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bnh.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gkc.birdmap.top

C#:   s.Replace("a", "b")
来源：http://yub.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://djo.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pgn.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nhu.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qli.ivvv.top

TS:   s.split(",")
来源：http://uzs.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://waj.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hsz.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://fof.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hqk.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://wzl.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://ztj.yongpay.top

PHP:  implode(",", $items);
来源：http://yvu.havefunace.top

JS:   items.join(",")
来源：http://kqb.zhixingplan.top

TS:   items.join(",")
来源：http://cbi.epnwcf.com

Java: String.join(",", items)
来源：http://lxe.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://gti.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://yvp.pycfn.com

C#:   string.Join(",", items)
来源：http://nys.0kj1m.cn

[E09] 去除所有空白字符
来源：http://cjl.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bdm.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oko.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ezc.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://rss.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://vft.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://voh.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lte.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lzk.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://vev.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hbo.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uur.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://pbb.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://ffb.yfazqb.com

Java: String.format("%03d", 7)
来源：http://gko.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ope.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jgj.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vzf.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://zoa.jinqigufen.top

Py:   s[::-1]
来源：http://fus.cdnleiting.top

PHP:  strrev($s);
来源：http://ekp.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://vxf.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://hwa.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://raa.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vco.hnxiangtu.top

Ruby: s.reverse
来源：http://xap.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://tlq.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://zjk.epnwcf.com

Py:   s.count("a")
来源：http://wan.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://lnv.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://mzo.vehdjk.com

TS:   s.split("a").length - 1
来源：http://nja.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://srh.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://gzl.sweek.top

Ruby: s.count("a")
来源：http://gav.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://njh.tanke756.top

[E13] 逐字符遍历
来源：http://rzp.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://sxv.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://opm.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jrw.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://wjj.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://npi.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tze.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yem.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hfl.xinyue.icu

[E14] URL 编码与 Base64
来源：http://duv.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ech.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ngf.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wfi.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rbh.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mfy.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vus.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xry.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lmf.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://xgl.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lya.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iwy.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ura.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mey.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jfv.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyw.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fbl.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pht.c1oappe.top

[E16] 数字千分位
来源：http://zxa.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://hmy.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://gry.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ane.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://uhi.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cwn.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qei.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ukz.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://qna.aibaodan.cn

[E17] 首字母大写
来源：http://ltk.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aej.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zog.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xcu.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zhl.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nxf.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bud.uphjek.com

Ruby: s.capitalize
来源：http://vqd.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ksi.yuanzhike.top


<!-- 参考信息 -->