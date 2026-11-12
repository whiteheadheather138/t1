代发 wailian999

TS:   [...arr].reverse();
来源：http://htz.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://geq.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://bsw.sysykeji.top

Ruby: arr.reverse
来源：http://ogi.yuanzhike.top

C#:   list.Reverse();
来源：http://kcy.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://avd.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://jvv.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hzl.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ucp.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lkx.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qvy.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://kmd.jlsjyb.cn

Ruby: arr.index(x)
来源：http://jst.hesvh.cn

C#:   list.IndexOf(x);
来源：http://pbj.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://jlz.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://acw.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ctm.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://dbf.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://pbr.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wim.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wzc.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://miq.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tcq.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://ojb.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ciq.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wnf.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://wjt.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://efp.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wbo.chenzaomai.com

Go:   // 手写循环
来源：http://wqw.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://abk.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://wcw.chenzaomai.com

[D15] 去重
来源：http://jnv.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pds.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://hgz.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://gus.fehbvm.com

TS:   [...new Set(arr)]
来源：http://ubj.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lax.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://wch.yangfankeji.com

Ruby: arr.uniq
来源：http://lin.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://dap.cashguo.top

[D16] 求和与平均值
来源：http://fqe.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghi.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://naq.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nlc.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sal.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pua.yuanzhike.top

Go:   // 手写循环累加
来源：http://peu.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ejy.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://kuy.uphjek.com

[D17] 最大值与最小值
来源：http://ckh.yonumen.top

Py:   max(arr);  min(arr)
来源：http://kkm.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://qak.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bkl.cheryme.top

TS:   Math.max(...arr);
来源：http://vkv.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nwe.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bql.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://nia.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://cke.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://ehc.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jbq.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://mgm.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xta.cqqwz.cn

TS:   nested.flat();
来源：http://aeq.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vxq.bbcook.cn

Go:   // 手写双层循环
来源：http://fro.iojbl.cn

Ruby: nested.flatten
来源：http://kjj.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zda.xinyue.icu

[D19] 按字段分组
来源：http://lfe.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bhq.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vze.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qiw.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rix.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://txx.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://zhu.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qag.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zju.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://mmz.dashuyun.cn

Py:   Counter(arr)
来源：http://ukm.xziqi.cn

PHP:  array_count_values($arr);
来源：http://zoq.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pnr.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iim.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ehv.xylfe.cn

Go:   // 手写 map[T]int
来源：http://mpq.dianchejie.cn

Ruby: arr.tally
来源：http://bbq.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ueh.epnwcf.com

[D21] 判断是否包含某元素
来源：http://kaf.yuanzhike.top

Py:   x in arr
来源：http://vio.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://dxz.sufxvd.cn

JS:   arr.includes(x)
来源：http://ugg.ybcxt.top

TS:   arr.includes(x)
来源：http://brz.gzhubu.top

Java: list.contains(x)
来源：http://wza.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://mok.chenlongwang.top

Ruby: arr.include?(x)
来源：http://vgb.chenlongwang.top

C#:   list.Contains(x)
来源：http://adi.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://kou.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zoi.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kmr.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://opd.jiagoushi.top

TS:   [...arr];
来源：http://nci.hcnkem.com

Java: new ArrayList<>(list);
来源：http://jor.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://kkh.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://nof.hammf.cn

C#:   new List<int>(list);
来源：http://kzm.shuidangran.top

[D23] reduce 累积计算
来源：http://har.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wuy.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dxc.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ytq.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hrm.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rdq.zhoulong.xyz

Go:   // 手写循环
来源：http://zcc.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kvq.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cqq.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://osx.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hwc.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iay.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jas.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oqn.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ogm.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://caa.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dag.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gbj.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://fcl.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ltb.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ufp.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ybw.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hdc.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tok.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://quo.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yvd.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bef.yuxming.cn

[D26] 数组转字符串
来源：http://tvj.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://juv.tanke756.top

PHP:  implode(", ", $arr);
来源：http://zak.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://fey.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://tsm.bjfxy.top

Java: String.join(", ", list)
来源：http://rwv.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://bnc.xziqi.cn

Ruby: arr.join(", ")
来源：http://joo.smart0.xyz

C#:   string.Join(", ", list)
来源：http://hrj.feifeiyinyue.top

================================================================================
来源：http://vmm.jqgufenzy.top

E. 字符串处理
来源：http://agr.fengsongda.top

================================================================================
来源：http://eqa.snrcjt.cn

[E01] 拼接字符串
来源：http://yvt.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vps.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zwq.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://icd.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vmi.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eci.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hct.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://asv.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qmd.ctjpmb.com

[E02] 重复字符串
来源：http://azy.fengsongda.top

Py:   "ab" * 3
来源：http://ist.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://bwf.nwbrower.top

JS:   "ab".repeat(3)
来源：http://yjq.ybcxt.top

TS:   "ab".repeat(3)
来源：http://pok.gogol.net.cn

Java: "ab".repeat(3)
来源：http://kuq.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://uwg.zdqjudy.top

Ruby: "ab" * 3
来源：http://kld.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yfd.ybcxt.top

[E03] 截取子串
来源：http://fcy.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ouv.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rtc.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cdw.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://zfz.pycfn.com

Java: s.substring(1, 4)
来源：http://oki.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://okv.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://plf.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://ozb.gogol.net.cn

[E04] 查找子串位置
来源：http://chd.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://qst.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://kme.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vpl.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://hsd.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://vbi.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://mqa.fehbvm.com

Ruby: s.index("x")
来源：http://qdn.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://fzc.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dxn.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://exu.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xhe.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fza.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://hyz.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjd.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uiu.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lay.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mry.cucudq.cn

[E06] 替换子串
来源：http://bjy.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kev.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://hfa.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://drn.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://ssu.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tyd.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kps.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vra.havefunace.top

C#:   s.Replace("a", "b")
来源：http://rrd.nanxinkj.top

[E07] 按分隔符拆分
来源：http://kpp.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rwk.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpf.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yje.cdnleiting.top

TS:   s.split(",")
来源：http://gyr.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dkj.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kks.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://kgn.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mlc.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://tyd.sxryk.cn

Py:   ",".join(items)
来源：http://ppa.jqgfzy.top

PHP:  implode(",", $items);
来源：http://pqc.hongshengwenyu.top

JS:   items.join(",")
来源：http://tlz.guowangkeji.top

TS:   items.join(",")
来源：http://lif.jianghu66.top

Java: String.join(",", items)
来源：http://noq.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://ohz.cqqwz.cn

Ruby: items.join(",")
来源：http://pks.chenzaomai.com

C#:   string.Join(",", items)
来源：http://uye.tian-w.cn

[E09] 去除所有空白字符
来源：http://yuq.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cnc.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sxp.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://njz.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://eiq.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://pla.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://olg.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://xcs.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jfb.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://dtm.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://arl.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uqx.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://kop.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://sfb.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://exm.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qfn.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ghh.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tvu.wangshuangyany.cn

[E11] 反转字符串
来源：http://fdi.ehwqpu.com

Py:   s[::-1]
来源：http://bli.yj20258888.top

PHP:  strrev($s);
来源：http://jkt.cashguo.top

JS:   [...s].reverse().join("")
来源：http://hia.tanke756.top

TS:   [...s].reverse().join("")
来源：http://yvp.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wlf.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oxv.hammf.cn

Ruby: s.reverse
来源：http://nql.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uxb.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://ehw.hcnkem.com

Py:   s.count("a")
来源：http://blf.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://omy.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://qad.ydzc1.top

TS:   s.split("a").length - 1
来源：http://ypl.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iqs.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://yqz.9152youxi.cn

Ruby: s.count("a")
来源：http://akv.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://lbz.zdqjudy.top

[E13] 逐字符遍历
来源：http://mpk.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://ckd.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eof.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://thz.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gxk.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mry.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mgb.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mme.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ynr.cheryme.top

[E14] URL 编码与 Base64
来源：http://meu.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://grz.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ure.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://neb.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lpy.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://btb.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sco.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tiw.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sth.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://hkw.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ldd.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://psc.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dhz.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uyz.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vkb.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uzj.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://och.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmf.nwbrower.top

[E16] 数字千分位
来源：http://wyp.redwolf501.top

Py:   f"{1234567:,}"
来源：http://dvf.chenzaomai.com

PHP:  number_format(1234567);
来源：http://zwn.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bsg.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://twp.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pxu.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yhn.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqm.cheryme.top

C#:   1234567.ToString("N0")
来源：http://ihp.zdbjq.cn

[E17] 首字母大写
来源：http://yhv.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uec.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fsy.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvf.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkz.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qkf.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iup.yj20258888.top

Ruby: s.capitalize
来源：http://yid.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ula.sysykeji.top

[E18] 模板占位符替换
来源：http://sfj.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kor.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xth.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oaj.xinyue.icu


<!-- 参考信息 -->