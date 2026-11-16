代发 wailian999

Ruby: arr.index(x)
来源：http://gig.cheryme.top

C#:   list.IndexOf(x);
来源：http://vec.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://lik.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mgj.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://csf.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://dkf.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://xsd.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bas.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cow.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://uam.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zvc.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://brb.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ggj.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vky.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://uhp.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://irw.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lfb.gzhubu.top

Go:   // 手写循环
来源：http://vda.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://pdb.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xyf.yj202588.top

[D15] 去重
来源：http://qrk.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mwy.uphjek.com

PHP:  array_unique($arr);
来源：http://gip.epnwcf.com

JS:   [...new Set(arr)]
来源：http://qrs.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://ogn.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vjy.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://efk.yvedp.cn

Ruby: arr.uniq
来源：http://pjx.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://jgl.shzxlz.cn

[D16] 求和与平均值
来源：http://lbh.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oct.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iko.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tey.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bjq.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofp.hysaishi.cn

Go:   // 手写循环累加
来源：http://fnz.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rwb.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://qyr.yuxming.cn

[D17] 最大值与最小值
来源：http://ffg.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://lsc.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://ldp.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qrk.vehdjk.com

TS:   Math.max(...arr);
来源：http://wgw.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://awa.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tkv.tarul.cn

Ruby: arr.max;  arr.min
来源：http://nit.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://ksb.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://yzm.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bus.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://xpz.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fxp.hammf.cn

TS:   nested.flat();
来源：http://dpy.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yqm.yuxming.cn

Go:   // 手写双层循环
来源：http://ywk.0kj1m.cn

Ruby: nested.flatten
来源：http://ljl.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lry.shangyingyoupin.top

[D19] 按字段分组
来源：http://xwf.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jny.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://btq.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jlj.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fcc.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dkd.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://diq.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sql.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mvg.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://qkp.fengsongda.top

Py:   Counter(arr)
来源：http://lzv.uphjek.com

PHP:  array_count_values($arr);
来源：http://rho.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bkn.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ufw.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vgm.xylfe.cn

Go:   // 手写 map[T]int
来源：http://mdw.cheryme.top

Ruby: arr.tally
来源：http://pqd.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zfz.wangdashe.top

[D21] 判断是否包含某元素
来源：http://niq.xuetiantiany.cn

Py:   x in arr
来源：http://tne.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://lhm.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://qbh.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://uuz.shanyushiyangtech.top

Java: list.contains(x)
来源：http://iyp.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://gzu.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://hol.smart0.xyz

C#:   list.Contains(x)
来源：http://bkg.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://caj.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mcy.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kod.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tjf.yueranfly.top

TS:   [...arr];
来源：http://bat.hcnkem.com

Java: new ArrayList<>(list);
来源：http://wdq.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://nlu.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://kim.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://ykk.kuanghao11.cn

[D23] reduce 累积计算
来源：http://pza.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eye.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ysl.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njy.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hqv.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xzs.zhiwuduotai.top

Go:   // 手写循环
来源：http://qbm.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nru.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nnh.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://tgy.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://una.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ccy.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbx.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vot.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://plf.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lld.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsj.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ruo.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://fih.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vie.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yse.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://upp.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kcz.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qlz.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://axz.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fov.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ume.yueranfly.top

[D26] 数组转字符串
来源：http://cmn.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://yyo.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://kmg.zhixingplan.top

JS:   arr.join(", ")
来源：http://sxm.jinqigfzy.top

TS:   arr.join(", ")
来源：http://qlk.bjfxy.top

Java: String.join(", ", list)
来源：http://xbk.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://khb.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://lkq.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://rdc.xinyue.icu

================================================================================
来源：http://jyo.yonumen.top

E. 字符串处理
来源：http://qbf.jiagoushi.top

================================================================================
来源：http://gmv.nanxuanxn.top

[E01] 拼接字符串
来源：http://zpa.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mgx.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ams.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wod.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dbm.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fkt.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pog.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://szi.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ego.yfazqb.com

[E02] 重复字符串
来源：http://axs.xziqi.cn

Py:   "ab" * 3
来源：http://ihs.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://xfa.cucudq.cn

JS:   "ab".repeat(3)
来源：http://jwm.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://qne.gotoacloud.top

Java: "ab".repeat(3)
来源：http://mxd.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://siv.bbcook.cn

Ruby: "ab" * 3
来源：http://gbs.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cci.zhiwuduotai.top

[E03] 截取子串
来源：http://pbl.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ggk.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xcj.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fjp.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://lvr.zhengqikj.top

Java: s.substring(1, 4)
来源：http://uui.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vvc.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://vcz.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://okg.daria6918.cn

[E04] 查找子串位置
来源：http://ufx.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://wbc.ydzc1.top

PHP:  strpos($s, "x");
来源：http://ymz.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zrd.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://fgc.jiagoushi.top

Java: s.indexOf("x")
来源：http://znq.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://ahf.yvedp.cn

Ruby: s.index("x")
来源：http://fek.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://ecr.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ibh.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vgh.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://muj.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fqv.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://evh.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gfk.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://usd.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://evl.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uur.quarkkingdee.top

[E06] 替换子串
来源：http://iht.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ssb.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://der.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://diw.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://dnn.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rib.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xdb.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://glg.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://eua.uphjek.com

[E07] 按分隔符拆分
来源：http://pjk.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ngj.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aom.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pjf.tanke756.top

TS:   s.split(",")
来源：http://aus.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://cas.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vcg.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://tyb.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lgc.jianghu66.top

[E08] 数组按分隔符合并
来源：http://opy.redwolf501.top

Py:   ",".join(items)
来源：http://bys.zycfv.cn

PHP:  implode(",", $items);
来源：http://qvw.shanyushiyangtech.top

JS:   items.join(",")
来源：http://std.gzhubu.top

TS:   items.join(",")
来源：http://ayw.wangdashe.top

Java: String.join(",", items)
来源：http://auo.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://ehh.fktsv.cn

Ruby: items.join(",")
来源：http://ajx.andypj.xyz

C#:   string.Join(",", items)
来源：http://isy.zhengqikj.top

[E09] 去除所有空白字符
来源：http://rcj.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ivc.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uww.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://owj.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://bhg.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://sgl.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ose.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://pvl.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ilp.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://gsv.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fdk.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rsy.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://ema.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://ysd.316326.xyz

Java: String.format("%03d", 7)
来源：http://qhe.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jox.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jwp.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://znt.52xcode.cn

[E11] 反转字符串
来源：http://epj.jinghuilouyu.cn

Py:   s[::-1]
来源：http://zef.yangfankeji.com

PHP:  strrev($s);
来源：http://tss.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://rqi.yj202588.top

TS:   [...s].reverse().join("")
来源：http://ojv.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gnn.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ono.bjfxy.top

Ruby: s.reverse
来源：http://efk.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://puc.iojbl.cn

[E12] 统计某字符出现次数
来源：http://goy.fktsv.cn

Py:   s.count("a")
来源：http://mav.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://fai.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://wfu.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://pio.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mnl.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://ffo.fengsongda.top

Ruby: s.count("a")
来源：http://qza.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://kvm.ppjwa.cn

[E13] 逐字符遍历
来源：http://djj.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://bfo.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gcd.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iiy.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ioc.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ult.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://njf.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wuk.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://obp.fehbvm.com

[E14] URL 编码与 Base64
来源：http://rdh.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ske.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ywj.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pyl.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oxt.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ecs.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kix.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xcj.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rda.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://nbg.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://die.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ybg.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zea.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ysj.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://brc.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fxg.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yvj.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://thd.sweek.top

[E16] 数字千分位
来源：http://etd.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://yqk.cdnleiting.top

PHP:  number_format(1234567);
来源：http://lrw.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vdz.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hcy.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ere.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vzs.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hos.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://iiv.hammf.cn

[E17] 首字母大写
来源：http://nff.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mau.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oaa.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkx.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xlo.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmi.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://asi.sysykeji.top

Ruby: s.capitalize
来源：http://yug.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://krt.yj20258888.top

[E18] 模板占位符替换
来源：http://bns.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wfp.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hiv.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gxx.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kef.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xke.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iwy.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jdd.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xkm.tanke756.top

[E19] 多行文本按行拆分
来源：http://lfa.kuanghao11.cn

Py:   s.splitlines()
来源：http://ora.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://azk.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://chp.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://pqp.316326.xyz

Java: s.lines().toList()
来源：http://ylv.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://qcg.hcnkem.com


<!-- 参考信息 -->