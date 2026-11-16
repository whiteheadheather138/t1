代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uzo.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://cpr.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://rax.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jkt.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oez.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pon.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://gyu.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://zxy.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tvf.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yvr.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://lef.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://drb.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vav.yvedp.cn

Go:   // 手写循环
来源：http://rnr.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uud.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fql.zhongyouzk.top

[D15] 去重
来源：http://noz.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ecz.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://dpc.xylfe.cn

JS:   [...new Set(arr)]
来源：http://tnc.xinyue.icu

TS:   [...new Set(arr)]
来源：http://jkb.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wva.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ggd.bbcook.cn

Ruby: arr.uniq
来源：http://htg.meibo888.top

C#:   list.Distinct().ToList()
来源：http://bml.haohaochexian.top

[D16] 求和与平均值
来源：http://ril.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iyl.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://its.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yon.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://spx.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kqe.zdqjudy.top

Go:   // 手写循环累加
来源：http://ykc.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wzn.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://ucl.vqdsnc.cn

[D17] 最大值与最小值
来源：http://lkq.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://qht.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://hyx.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pza.c1oappe.top

TS:   Math.max(...arr);
来源：http://jnt.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://upo.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://whr.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://mml.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://lim.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://cby.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blr.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://mjf.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kyk.9152youxi.cn

TS:   nested.flat();
来源：http://tag.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yto.tanke756.top

Go:   // 手写双层循环
来源：http://fbx.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://cps.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://exp.sxryk.cn

[D19] 按字段分组
来源：http://nlp.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qsi.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vyl.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fln.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jnt.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzm.tarul.cn

Go:   // 手写 map[string][]T
来源：http://rlh.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wlp.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gnp.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://vmc.316326.xyz

Py:   Counter(arr)
来源：http://nbj.shuidangran.top

PHP:  array_count_values($arr);
来源：http://buy.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ksy.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cix.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nvj.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://vxk.jlsjyb.cn

Ruby: arr.tally
来源：http://xtc.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ebx.fehbvm.com

[D21] 判断是否包含某元素
来源：http://euq.ctjpmb.com

Py:   x in arr
来源：http://wph.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://cpu.yuxming.cn

JS:   arr.includes(x)
来源：http://yaa.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://cbd.zdbjq.cn

Java: list.contains(x)
来源：http://map.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://fkg.52xcode.cn

Ruby: arr.include?(x)
来源：http://bmi.0kj1m.cn

C#:   list.Contains(x)
来源：http://lsa.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://bcr.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://svx.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ltc.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kia.xuanzx.com

TS:   [...arr];
来源：http://jki.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://jrm.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://oor.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://evc.c1oappe.top

C#:   new List<int>(list);
来源：http://vhu.andypj.xyz

[D23] reduce 累积计算
来源：http://hkn.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://elk.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ymw.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mrb.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dax.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uan.aibaodan.cn

Go:   // 手写循环
来源：http://gzc.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://khy.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yso.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://iqj.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yoq.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rta.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vkv.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ljs.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dsr.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nta.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wnw.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vnd.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://zus.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ros.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kjd.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xld.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://huy.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nlr.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://brv.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dzg.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vwr.fengsongda.top

[D26] 数组转字符串
来源：http://qsr.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://myz.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://eus.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://nww.zdbjq.cn

TS:   arr.join(", ")
来源：http://ibr.hywenlv.cn

Java: String.join(", ", list)
来源：http://wqx.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://ymt.tianlin.xyz

Ruby: arr.join(", ")
来源：http://qhp.yj20258888.top

C#:   string.Join(", ", list)
来源：http://blc.jinghuilouyu.cn

================================================================================
来源：http://flz.aibaodan.cn

E. 字符串处理
来源：http://koz.ppjwa.cn

================================================================================
来源：http://mox.zhengqikj.top

[E01] 拼接字符串
来源：http://lnq.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xrx.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gfv.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://czs.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgq.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jrc.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdn.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nah.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lai.kuanghao11.cn

[E02] 重复字符串
来源：http://uvj.kuanghao11.cn

Py:   "ab" * 3
来源：http://opl.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://tvl.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://sjy.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://imo.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://wfg.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://cqy.yueranfly.top

Ruby: "ab" * 3
来源：http://rre.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zll.52xcode.cn

[E03] 截取子串
来源：http://lfj.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymt.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vqr.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aao.52xcode.cn

TS:   s.slice(1, 4)
来源：http://bsy.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://ben.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://msm.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tkr.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://jpw.xuanzx.com

[E04] 查找子串位置
来源：http://vsc.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://agt.wangdashe.top

PHP:  strpos($s, "x");
来源：http://iez.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cor.gzhubu.top

TS:   s.indexOf("x")
来源：http://wao.yonumen.top

Java: s.indexOf("x")
来源：http://low.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://uuo.hnqzz.top

Ruby: s.index("x")
来源：http://iqg.yj20258.top

C#:   s.IndexOf("x")
来源：http://xfv.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zmj.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://opx.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tas.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fbw.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cvl.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://the.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jct.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kgv.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myi.fktsv.cn

[E06] 替换子串
来源：http://wgx.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ioa.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://kqu.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://soe.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://zsd.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fes.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://orh.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vza.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://mdo.wangdashe.top

[E07] 按分隔符拆分
来源：http://hbp.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wbj.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ajl.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://blr.zhongyouzk.top

TS:   s.split(",")
来源：http://quw.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rqn.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pxa.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://lef.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uyj.hnqzz.top

[E08] 数组按分隔符合并
来源：http://kyq.daria6918.cn

Py:   ",".join(items)
来源：http://yod.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://wyl.havefunace.top

JS:   items.join(",")
来源：http://tlz.smart0.xyz

TS:   items.join(",")
来源：http://zfk.xylfe.cn

Java: String.join(",", items)
来源：http://tgz.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://udu.tarul.cn

Ruby: items.join(",")
来源：http://eot.wangdashe.top

C#:   string.Join(",", items)
来源：http://plp.cdnleiting.top

[E09] 去除所有空白字符
来源：http://vkf.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://egr.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zct.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://mrx.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://iwf.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://ktw.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mky.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://ozc.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ewh.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://cmd.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bny.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dqn.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://fxx.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://gmg.iojbl.cn

Java: String.format("%03d", 7)
来源：http://eml.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://dqe.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nbq.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tcb.birdmap.top

[E11] 反转字符串
来源：http://qmz.jyoumei.cn

Py:   s[::-1]
来源：http://abw.yonumen.top

PHP:  strrev($s);
来源：http://xnw.havefunace.top

JS:   [...s].reverse().join("")
来源：http://jyn.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://fuz.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cjx.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ogw.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://mzk.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://jdp.sxryk.cn

[E12] 统计某字符出现次数
来源：http://eac.ydjk.org.cn

Py:   s.count("a")
来源：http://fkg.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://van.cucudq.cn

JS:   s.split("a").length - 1
来源：http://stz.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://jqa.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lmn.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://pvf.zdbjq.cn

Ruby: s.count("a")
来源：http://nyw.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://pqm.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://sjs.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://wzq.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xmn.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wkw.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mkf.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ewi.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ptz.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dox.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xxu.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://pbr.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hbn.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jyb.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://stk.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uos.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uob.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhm.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://riy.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gyv.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://zdx.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jvg.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://epd.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nip.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tiy.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gst.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tae.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zwz.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oir.yj202588.top

[E16] 数字千分位
来源：http://xin.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://kdh.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://asz.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fln.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rqs.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oap.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nqk.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uwf.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://alr.52xcode.cn

[E17] 首字母大写
来源：http://cqv.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pip.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rtl.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yjy.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbl.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aka.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zux.xuanzx.com

Ruby: s.capitalize
来源：http://iae.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://azd.epnwcf.com

[E18] 模板占位符替换
来源：http://skd.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zsj.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bjv.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kyh.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ykt.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://abo.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sqd.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fay.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wqe.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://yza.yj20258888.top

Py:   s.splitlines()
来源：http://gtd.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jiz.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://wpq.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://vkj.ivvv.top

Java: s.lines().toList()
来源：http://lhd.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://agc.fktsv.cn

Ruby: s.lines
来源：http://twl.ydjk.org.cn

C#:   s.Split('\n')
来源：http://kgc.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://lin.hnxiangtu.top

Py:   if not s:
来源：http://yzb.zhongyouzk.top


<!-- 参考信息 -->