代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mpq.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fwg.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iwc.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nhh.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cst.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tsl.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://irx.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ydb.9152youxi.cn

[D11] 反转数组
来源：http://zqv.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://ean.cheryme.top

PHP:  array_reverse($arr);
来源：http://ues.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxr.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://voi.yongpay.top

Java: Collections.reverse(list);
来源：http://bab.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://oav.0kj1m.cn

Ruby: arr.reverse
来源：http://dul.dianchejie.cn

C#:   list.Reverse();
来源：http://dhr.zdqjudy.top

[D12] 查找元素下标
来源：http://ydu.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://foz.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vtw.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ahp.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shx.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbo.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://uyg.fengsongda.top

Ruby: arr.index(x)
来源：http://zbd.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://dis.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://vow.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kwg.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dfn.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://sek.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://aay.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ppv.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qht.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yuy.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dit.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://vjr.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dso.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://syc.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://hgr.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://nmh.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://rlz.dianchejie.cn

Go:   // 手写循环
来源：http://has.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://grl.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uae.zhongyouzk.top

[D15] 去重
来源：http://xsn.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rko.sxryk.cn

PHP:  array_unique($arr);
来源：http://khq.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://aek.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://izv.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lpw.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nud.dashuyun.cn

Ruby: arr.uniq
来源：http://ijr.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://aiz.ydjk.org.cn

[D16] 求和与平均值
来源：http://aqm.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jsn.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://naq.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tvo.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzc.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cqw.sxryk.cn

Go:   // 手写循环累加
来源：http://wnp.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yxe.316326.xyz

C#:   list.Sum();  list.Average()
来源：http://ifb.hysaishi.cn

[D17] 最大值与最小值
来源：http://lqz.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://wfj.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://dya.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ldt.sweek.top

TS:   Math.max(...arr);
来源：http://qvp.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://rrg.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://arm.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://rpi.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://xle.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://pbx.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dak.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://hat.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://evk.0kj1m.cn

TS:   nested.flat();
来源：http://zrm.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gri.sweek.top

Go:   // 手写双层循环
来源：http://stp.jianghu66.top

Ruby: nested.flatten
来源：http://wvy.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmp.yangfankeji.com

[D19] 按字段分组
来源：http://mqo.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xwu.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hqc.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://opa.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ogf.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gri.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://ais.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://bte.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wxr.tarul.cn

[D20] 统计每个元素出现次数
来源：http://sfh.gotoacloud.top

Py:   Counter(arr)
来源：http://eij.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://vbw.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwu.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fth.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cyo.hcnkem.com

Go:   // 手写 map[T]int
来源：http://yrk.nwbrower.top

Ruby: arr.tally
来源：http://dfg.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xft.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://rhq.zhaomingkeji.xyz

Py:   x in arr
来源：http://mra.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://sja.shuidangran.top

JS:   arr.includes(x)
来源：http://grx.dashuyun.cn

TS:   arr.includes(x)
来源：http://ldj.vqdsnc.cn

Java: list.contains(x)
来源：http://hck.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://svp.ybcxt.top

Ruby: arr.include?(x)
来源：http://eyf.meibo888.top

C#:   list.Contains(x)
来源：http://qlt.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://bbt.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qfe.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ghk.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dja.yonumen.top

TS:   [...arr];
来源：http://zrm.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://zxm.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wau.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://tsw.guowangkeji.top

C#:   new List<int>(list);
来源：http://qmt.guowangkeji.top

[D23] reduce 累积计算
来源：http://knv.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpj.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wgl.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kam.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kjl.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fjz.hammf.cn

Go:   // 手写循环
来源：http://ebf.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://agh.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://syf.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://bdn.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nmw.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qrt.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://czo.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rjc.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iqx.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://trd.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tre.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wrs.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://xsi.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://irv.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pjy.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gbe.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dvc.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nah.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yls.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ehm.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tyk.ydjk.org.cn

[D26] 数组转字符串
来源：http://lfu.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://hgk.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://xcv.snrcjt.cn

JS:   arr.join(", ")
来源：http://fqs.bjfxy.top

TS:   arr.join(", ")
来源：http://efn.fzhhl.top

Java: String.join(", ", list)
来源：http://ysp.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://zzv.c1oappe.top

Ruby: arr.join(", ")
来源：http://nfi.ivvv.top

C#:   string.Join(", ", list)
来源：http://byk.zhongyouzk.top

================================================================================
来源：http://orf.fanxiaobao.xyz

E. 字符串处理
来源：http://lxi.aizwys.cn

================================================================================
来源：http://uqy.shangyingyoupin.top

[E01] 拼接字符串
来源：http://uag.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dvd.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eoq.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fxe.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uja.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qiy.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wqs.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oyf.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://teb.yj20258888.top

[E02] 重复字符串
来源：http://dbc.aibaodan.cn

Py:   "ab" * 3
来源：http://jwl.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://lvs.tian-w.cn

JS:   "ab".repeat(3)
来源：http://vzl.yvedp.cn

TS:   "ab".repeat(3)
来源：http://tgg.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://hou.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://zhq.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://kxc.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://buj.kuanghao11.cn

[E03] 截取子串
来源：http://vfg.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iku.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kng.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nfw.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://bqr.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://ppo.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gbj.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rvd.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://zgw.vehdjk.com

[E04] 查找子串位置
来源：http://bjz.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://clq.zycfv.cn

PHP:  strpos($s, "x");
来源：http://chy.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://njl.fktsv.cn

TS:   s.indexOf("x")
来源：http://nkz.yangfankeji.com

Java: s.indexOf("x")
来源：http://arm.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://ung.fktsv.cn

Ruby: s.index("x")
来源：http://dnm.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://mlc.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bcp.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lfn.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aqs.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxz.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hxx.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yqw.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zhy.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zlk.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ioo.ehwqpu.com

[E06] 替换子串
来源：http://atm.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://suy.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://tcu.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzw.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://gut.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eaq.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yso.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ltm.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://vlz.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://xyq.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://chb.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rgw.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zuh.52xcode.cn

TS:   s.split(",")
来源：http://rga.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://mez.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ulb.yj202588.top

Ruby: s.split(",");  s.split
来源：http://ulc.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gfr.hesvh.cn

[E08] 数组按分隔符合并
来源：http://fnb.jiagoushi.top

Py:   ",".join(items)
来源：http://ywv.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://dei.havefunace.top

JS:   items.join(",")
来源：http://dxz.dianchejie.cn

TS:   items.join(",")
来源：http://nhg.xinyue.icu

Java: String.join(",", items)
来源：http://cjm.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://lgv.fengsongda.top

Ruby: items.join(",")
来源：http://eqj.bjfxy.top

C#:   string.Join(",", items)
来源：http://vhh.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://nbm.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wcc.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fzc.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://vjv.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://xbc.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ene.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lgj.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://dhm.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nvj.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://vxm.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bwy.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pvt.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://znf.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://gxz.yonumen.top

Java: String.format("%03d", 7)
来源：http://yht.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kju.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ody.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hsf.jinqigfzy.top

[E11] 反转字符串
来源：http://gqe.zhijiandao.cn

Py:   s[::-1]
来源：http://lqx.quarkkingdee.top

PHP:  strrev($s);
来源：http://oet.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://joa.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://mvc.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://zgc.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://wli.quarkkingdee.top

Ruby: s.reverse
来源：http://euj.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qfr.cheryme.top

[E12] 统计某字符出现次数
来源：http://vqg.daria6918.cn

Py:   s.count("a")
来源：http://ifd.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://lji.shuidangran.top

JS:   s.split("a").length - 1
来源：http://qvo.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://lkr.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aoj.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://wio.hywenlv.cn

Ruby: s.count("a")
来源：http://zya.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://iga.hesvh.cn

[E13] 逐字符遍历
来源：http://jxg.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://unb.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hag.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jve.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uzg.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hqd.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afz.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kyq.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hra.xylfe.cn

[E14] URL 编码与 Base64
来源：http://grb.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uhm.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://txg.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ryg.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hpq.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mej.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iha.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ncf.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jpo.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://lfv.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bic.smart0.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eid.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://las.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nuy.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hra.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyd.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://orr.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ljy.zhijiandao.cn

[E16] 数字千分位
来源：http://hoc.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://kyw.sweek.top

PHP:  number_format(1234567);
来源：http://jpe.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vgl.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nvy.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhp.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ahf.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vjw.tanke756.top

C#:   1234567.ToString("N0")
来源：http://vwb.jiagoushi.top

[E17] 首字母大写
来源：http://hpo.jyoumei.cn


<!-- 参考信息 -->