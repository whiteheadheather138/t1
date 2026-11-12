代发 wailian999

[D11] 反转数组
来源：http://kzf.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://vys.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://xbd.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://izw.andypj.xyz

TS:   [...arr].reverse();
来源：http://yza.yj20258888.top

Java: Collections.reverse(list);
来源：http://wvt.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://jtj.hywenlv.cn

Ruby: arr.reverse
来源：http://ubk.yueranfly.top

C#:   list.Reverse();
来源：http://ayx.9152youxi.cn

[D12] 查找元素下标
来源：http://ude.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://xaf.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://esi.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tzn.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oyr.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ius.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://bxp.hesvh.cn

Ruby: arr.index(x)
来源：http://axe.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://wjm.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://bsu.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://izr.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ciq.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://tny.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://bkl.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gwk.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xev.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jog.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://muc.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://apj.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kkm.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lqb.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://khy.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://snh.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hgn.yanxiufei.cn

Go:   // 手写循环
来源：http://nwu.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://did.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://czh.bjfxy.top

[D15] 去重
来源：http://ekr.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rna.jqgfzy.top

PHP:  array_unique($arr);
来源：http://hee.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://sdm.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://wpf.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hcf.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fme.pengpengdd.cyou

Ruby: arr.uniq
来源：http://eoi.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://unz.vqdsnc.cn

[D16] 求和与平均值
来源：http://tvb.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blh.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://axd.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmj.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fcd.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ngp.iojbl.cn

Go:   // 手写循环累加
来源：http://shv.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tcm.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://dkn.bjfxy.top

[D17] 最大值与最小值
来源：http://sda.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://tgr.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://lyx.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://thy.yonumen.top

TS:   Math.max(...arr);
来源：http://tkc.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gwu.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://imh.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://xts.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://xyq.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://qcc.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jld.tarul.cn

PHP:  array_merge(...$nested);
来源：http://pky.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wnu.andypj.xyz

TS:   nested.flat();
来源：http://cwq.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iar.iojbl.cn

Go:   // 手写双层循环
来源：http://rrc.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://cws.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zhd.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://jvp.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dun.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pdn.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qoz.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kmc.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cen.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://ecd.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nsr.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://opp.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://rpy.yj202588.top

Py:   Counter(arr)
来源：http://mls.guannengcc.top

PHP:  array_count_values($arr);
来源：http://qkn.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zuv.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erc.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ajb.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://mgi.hcnkem.com

Ruby: arr.tally
来源：http://ecb.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fdm.sysykeji.top

[D21] 判断是否包含某元素
来源：http://zeo.daxiang520.top

Py:   x in arr
来源：http://swg.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://wln.nanxinkj.top

JS:   arr.includes(x)
来源：http://qhu.yueranfly.top

TS:   arr.includes(x)
来源：http://pzk.0kj1m.cn

Java: list.contains(x)
来源：http://hkm.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://mst.yvedp.cn

Ruby: arr.include?(x)
来源：http://vyc.jqgfzy.top

C#:   list.Contains(x)
来源：http://fin.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://xuo.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kan.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hvh.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qze.ywan-chungtsiang.top

TS:   [...arr];
来源：http://ifs.epnwcf.com

Java: new ArrayList<>(list);
来源：http://fyf.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ozt.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://zoz.aibaodan.cn

C#:   new List<int>(list);
来源：http://iwt.bjfxy.top

[D23] reduce 累积计算
来源：http://wta.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fsi.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bma.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wbt.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyr.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ert.jianghu66.top

Go:   // 手写循环
来源：http://nen.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzc.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bvr.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://ufb.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hvf.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rny.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ugl.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tyk.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bzd.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xud.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bkj.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ijm.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://seg.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yem.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ztd.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dmt.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gjf.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mvh.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sfo.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://niu.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fqg.xuetiantiany.cn

[D26] 数组转字符串
来源：http://ddp.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://mwo.meibo888.top

PHP:  implode(", ", $arr);
来源：http://tmq.meibo888.top

JS:   arr.join(", ")
来源：http://ykk.316326.xyz

TS:   arr.join(", ")
来源：http://why.52xcode.cn

Java: String.join(", ", list)
来源：http://pch.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://tlm.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://uim.bjfxy.top

C#:   string.Join(", ", list)
来源：http://hiq.cucudq.cn

================================================================================
来源：http://cvz.zhoulong.xyz

E. 字符串处理
来源：http://gld.uphjek.com

================================================================================
来源：http://cpj.cucudq.cn

[E01] 拼接字符串
来源：http://joe.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owm.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zwy.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bfi.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ccr.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://clm.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://goe.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lgy.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ohj.haohaochexian.top

[E02] 重复字符串
来源：http://erz.ctjpmb.com

Py:   "ab" * 3
来源：http://xxd.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://fpf.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://zyi.zycfv.cn

TS:   "ab".repeat(3)
来源：http://uhx.52xcode.cn

Java: "ab".repeat(3)
来源：http://qit.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://kof.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://qem.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pnj.sweek.top

[E03] 截取子串
来源：http://wyg.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vip.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hdq.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkb.yj20258888.top

TS:   s.slice(1, 4)
来源：http://cuu.hfpthk.cn

Java: s.substring(1, 4)
来源：http://tdd.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nfi.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://nds.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://rai.cheryme.top

[E04] 查找子串位置
来源：http://bap.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://lfu.iojbl.cn

PHP:  strpos($s, "x");
来源：http://bwf.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mla.sxryk.cn

TS:   s.indexOf("x")
来源：http://rlp.vehdjk.com

Java: s.indexOf("x")
来源：http://exy.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://nap.xuetiantiany.cn

Ruby: s.index("x")
来源：http://ibi.smart0.xyz

C#:   s.IndexOf("x")
来源：http://cnu.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qqw.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ltg.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axw.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mou.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hsm.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://laz.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://onb.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hqq.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vmh.snrcjt.cn

[E06] 替换子串
来源：http://div.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tdo.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://pmw.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://spz.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://loq.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gip.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bky.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://opp.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://bkf.fzhhl.top

[E07] 按分隔符拆分
来源：http://fqz.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://swl.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fca.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://drx.sjlbkw.cn

TS:   s.split(",")
来源：http://ssf.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ihw.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dyf.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://ftl.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jew.xuanzx.com

[E08] 数组按分隔符合并
来源：http://moc.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://ute.yangfankeji.com

PHP:  implode(",", $items);
来源：http://mqq.xuetiantiany.cn

JS:   items.join(",")
来源：http://rfa.svipenyu.cn

TS:   items.join(",")
来源：http://jxz.hfpthk.cn

Java: String.join(",", items)
来源：http://kce.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://qwo.svipenyu.cn

Ruby: items.join(",")
来源：http://yjc.0kj1m.cn

C#:   string.Join(",", items)
来源：http://tnr.meibo888.top

[E09] 去除所有空白字符
来源：http://svg.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://stk.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nyu.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://ytn.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://zsl.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ezv.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ipj.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://vzx.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ifw.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://wob.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yzr.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://scn.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://dvy.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://erc.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://seo.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qtu.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oeo.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rgi.mhx1999.top

[E11] 反转字符串
来源：http://vaz.aizwys.cn

Py:   s[::-1]
来源：http://jbw.tarul.cn

PHP:  strrev($s);
来源：http://cri.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://uwr.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://akk.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yhd.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ysk.bjfxy.top

Ruby: s.reverse
来源：http://epk.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://vdl.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://fmh.xinyue.icu

Py:   s.count("a")
来源：http://emp.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://cnl.aizwys.cn

JS:   s.split("a").length - 1
来源：http://qcq.daria6918.cn

TS:   s.split("a").length - 1
来源：http://idx.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lha.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://vju.feifeiyinyue.top

Ruby: s.count("a")
来源：http://bta.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://qdx.9152youxi.cn

[E13] 逐字符遍历
来源：http://cvf.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://fkr.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kwi.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fsw.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lfb.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://czc.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ixw.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lvr.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pgn.mhx1999.top

[E14] URL 编码与 Base64
来源：http://ehv.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dfk.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mnh.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://awj.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gro.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gbs.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ecw.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kmx.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://azy.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://qip.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yop.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zkv.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hng.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://alm.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kkn.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cbk.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bhz.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gkc.zycfv.cn

[E16] 数字千分位
来源：http://ioa.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://zhj.9152youxi.cn

PHP:  number_format(1234567);
来源：http://txz.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wvh.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ncl.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iho.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vpc.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yki.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://zyt.bbcook.cn

[E17] 首字母大写
来源：http://ijy.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mnk.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ghu.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfy.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://enr.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ufz.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dkl.ivvv.top

Ruby: s.capitalize
来源：http://pns.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pxr.wangdashe.top


<!-- 参考信息 -->