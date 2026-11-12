代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ntc.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zfz.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qpv.havefunace.top

Go:   slices.Index(arr, x)
来源：http://tlo.hcnkem.com

Ruby: arr.index(x)
来源：http://oqj.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://nuf.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://psh.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xzl.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idd.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://kjo.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://men.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://htb.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bjs.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://gdx.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yer.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://vvm.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nuf.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zwz.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://kbf.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://swi.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://jca.andypj.xyz

Go:   // 手写循环
来源：http://qfi.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://uut.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hro.316326.xyz

[D15] 去重
来源：http://ziv.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wfb.ybcxt.top

PHP:  array_unique($arr);
来源：http://xub.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://gwi.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://jkv.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hri.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rmk.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://ndx.yongpay.top

C#:   list.Distinct().ToList()
来源：http://oue.52xcode.cn

[D16] 求和与平均值
来源：http://brx.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://poe.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tcx.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dos.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ijr.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tza.yuanzhike.top

Go:   // 手写循环累加
来源：http://jfu.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blm.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://ikk.zhoulong.xyz

[D17] 最大值与最小值
来源：http://pzd.yj202588.top

Py:   max(arr);  min(arr)
来源：http://fvv.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://dze.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ahz.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://iox.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mpb.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qpx.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://kqp.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://mzd.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://cen.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cqn.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://xtu.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://whk.uphjek.com

TS:   nested.flat();
来源：http://elj.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://use.chenzaomai.com

Go:   // 手写双层循环
来源：http://sxm.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://qff.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://plb.jinqigufen.top

[D19] 按字段分组
来源：http://owd.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://djp.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cci.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cpa.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dyh.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sjf.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://gep.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jjg.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nhy.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://pnn.fktsv.cn

Py:   Counter(arr)
来源：http://mwq.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://ihn.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ovj.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsi.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oln.epnwcf.com

Go:   // 手写 map[T]int
来源：http://xca.316326.xyz

Ruby: arr.tally
来源：http://acw.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://daq.xziqi.cn

[D21] 判断是否包含某元素
来源：http://ixn.jinghuilouyu.cn

Py:   x in arr
来源：http://gqy.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://jxj.xinyue.icu

JS:   arr.includes(x)
来源：http://qgn.xylfe.cn

TS:   arr.includes(x)
来源：http://jnd.xziqi.cn

Java: list.contains(x)
来源：http://whv.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://jjl.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://hqf.chenzaomai.com

C#:   list.Contains(x)
来源：http://nrq.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://jke.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mvr.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://khp.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pyy.zdbjq.cn

TS:   [...arr];
来源：http://wby.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://boc.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://sny.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://cgg.ctjpmb.com

C#:   new List<int>(list);
来源：http://fwm.cqqwz.cn

[D23] reduce 累积计算
来源：http://lxl.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pcc.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zbs.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxb.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqn.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ssq.yonumen.top

Go:   // 手写循环
来源：http://fix.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jgk.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ncm.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://ptc.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fga.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dva.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ozn.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qzs.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ree.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ovj.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lvh.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvn.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://zin.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cut.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tcr.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpy.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dsl.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pww.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ooh.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bkv.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mwk.zdbjq.cn

[D26] 数组转字符串
来源：http://whe.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://aiq.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://nhi.pycfn.com

JS:   arr.join(", ")
来源：http://sod.fktsv.cn

TS:   arr.join(", ")
来源：http://vxd.guannengcc.top

Java: String.join(", ", list)
来源：http://icf.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://kxc.c1oappe.top

Ruby: arr.join(", ")
来源：http://qng.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://bng.ydjk.org.cn

================================================================================
来源：http://viu.jinghuilouyu.cn

E. 字符串处理
来源：http://lji.guannengcc.top

================================================================================
来源：http://iii.yueranfly.top

[E01] 拼接字符串
来源：http://jcz.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wtk.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fhk.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://meh.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://woh.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dan.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aay.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://okq.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bpi.fktsv.cn

[E02] 重复字符串
来源：http://tzq.yj202588.top

Py:   "ab" * 3
来源：http://oar.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://jas.cucudq.cn

JS:   "ab".repeat(3)
来源：http://nfx.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://nos.ppjwa.cn

Java: "ab".repeat(3)
来源：http://tdt.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://knr.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://rjs.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fad.jinqigfzy.top

[E03] 截取子串
来源：http://hdm.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kzj.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aai.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kvn.yueranfly.top

TS:   s.slice(1, 4)
来源：http://wre.haohaochexian.top

Java: s.substring(1, 4)
来源：http://qil.dianchejie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dld.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://wfi.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://jcg.xinyue.icu

[E04] 查找子串位置
来源：http://gki.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://exi.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://thl.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://asm.xuanzx.com

TS:   s.indexOf("x")
来源：http://mnu.xinyue.icu

Java: s.indexOf("x")
来源：http://rmr.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://rxq.ctjpmb.com

Ruby: s.index("x")
来源：http://rxr.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://qdq.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lab.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ssg.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnr.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tow.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://det.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uwk.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://chs.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gky.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://svw.shanyushiyangkeji.top

[E06] 替换子串
来源：http://xte.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mgj.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://ggi.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://abt.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://ykv.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rvk.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uzg.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://duy.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://icd.cdnleiting.top

[E07] 按分隔符拆分
来源：http://bof.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mrt.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wmv.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mnh.tanke756.top

TS:   s.split(",")
来源：http://hab.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cub.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kiy.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://cqg.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dnc.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://dih.hfpthk.cn

Py:   ",".join(items)
来源：http://qni.sufxvd.cn

PHP:  implode(",", $items);
来源：http://feh.9152youxi.cn

JS:   items.join(",")
来源：http://nie.smart0.xyz

TS:   items.join(",")
来源：http://nng.chenlongwang.top

Java: String.join(",", items)
来源：http://meu.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://ahf.tarul.cn

Ruby: items.join(",")
来源：http://txq.zycfv.cn

C#:   string.Join(",", items)
来源：http://got.cashguo.top

[E09] 去除所有空白字符
来源：http://dce.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xuy.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fxk.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://lsw.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://gws.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://zpb.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nxz.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://udx.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mbn.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://raw.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ptj.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tmn.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://hbh.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://jeg.cucudq.cn

Java: String.format("%03d", 7)
来源：http://vyn.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://asx.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tih.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rgr.guowangkeji.top

[E11] 反转字符串
来源：http://xsd.chenlongwang.top

Py:   s[::-1]
来源：http://xhf.ehwqpu.com

PHP:  strrev($s);
来源：http://cvc.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://rcj.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://kry.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uyq.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dhb.shangyingyoupin.top

Ruby: s.reverse
来源：http://eod.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://vuw.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://qga.epnwcf.com

Py:   s.count("a")
来源：http://aji.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://qbp.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://kog.daria6918.cn

TS:   s.split("a").length - 1
来源：http://htz.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehk.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://rzd.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://trp.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://znl.cheryme.top

[E13] 逐字符遍历
来源：http://utk.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://upp.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ell.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://rke.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://etx.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vow.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yfi.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zek.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://btl.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://lzk.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sdw.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://gpr.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dch.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gwn.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vgh.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eix.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kwl.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxb.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://eqy.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bdb.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://olq.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://epe.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pgl.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vlp.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://avh.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aky.9152youxi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfo.xylfe.cn

[E16] 数字千分位
来源：http://ioi.tanke756.top

Py:   f"{1234567:,}"
来源：http://rza.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://mas.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gan.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jnu.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://obf.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xdk.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://giu.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://mba.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://vvf.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zou.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rmk.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uwz.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmc.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ygp.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://boz.uphjek.com

Ruby: s.capitalize
来源：http://irf.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://itd.daxiang520.top

[E18] 模板占位符替换
来源：http://acx.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://inw.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://slc.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://msb.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xry.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gql.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qgz.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cxv.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dut.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://dqm.chenzaomai.com

Py:   s.splitlines()
来源：http://ycl.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oyh.andypj.xyz


<!-- 参考信息 -->