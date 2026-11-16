代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xgx.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://drf.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gax.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://zyv.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dqg.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kre.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://jsp.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://emk.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgs.fktsv.cn

Go:   // 手写循环
来源：http://heg.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wkx.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://clo.sysykeji.top

[D15] 去重
来源：http://bhe.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://teg.zycfv.cn

PHP:  array_unique($arr);
来源：http://fmm.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://qsd.smart0.xyz

TS:   [...new Set(arr)]
来源：http://kgh.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yfm.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hsq.iojbl.cn

Ruby: arr.uniq
来源：http://lig.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://fxv.sxryk.cn

[D16] 求和与平均值
来源：http://bxz.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dst.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hif.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sfr.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://krl.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zdc.sxryk.cn

Go:   // 手写循环累加
来源：http://bey.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jua.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://wzc.gzhubu.top

[D17] 最大值与最小值
来源：http://vgm.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://ior.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://khl.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://byl.shuidangran.top

TS:   Math.max(...arr);
来源：http://aet.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mtl.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nvc.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://zzp.tarul.cn

C#:   list.Max();  list.Min()
来源：http://elv.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://afp.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sfh.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://hhg.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://idj.shuidangran.top

TS:   nested.flat();
来源：http://hxq.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rso.kuanghao11.cn

Go:   // 手写双层循环
来源：http://cer.yuxming.cn

Ruby: nested.flatten
来源：http://puc.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfu.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://wde.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://klg.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oxm.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bwm.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dew.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kag.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://lvg.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ten.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zaa.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://fjd.xinyue.icu

Py:   Counter(arr)
来源：http://rdy.andypj.xyz

PHP:  array_count_values($arr);
来源：http://pfl.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qie.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://htx.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vkc.ydzc1.top

Go:   // 手写 map[T]int
来源：http://mas.fktsv.cn

Ruby: arr.tally
来源：http://uhu.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eiw.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://iuz.hesvh.cn

Py:   x in arr
来源：http://skp.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://pba.snrcjt.cn

JS:   arr.includes(x)
来源：http://ajl.guannengcc.top

TS:   arr.includes(x)
来源：http://qjj.jinqigfzy.top

Java: list.contains(x)
来源：http://mrv.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://yte.hysaishi.cn

Ruby: arr.include?(x)
来源：http://wuh.fengsongda.top

C#:   list.Contains(x)
来源：http://lyi.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://aop.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vkr.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ifo.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dsh.ctjpmb.com

TS:   [...arr];
来源：http://lnp.meibo888.top

Java: new ArrayList<>(list);
来源：http://cip.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dys.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://wml.uphjek.com

C#:   new List<int>(list);
来源：http://vaw.52xcode.cn

[D23] reduce 累积计算
来源：http://ddi.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ydt.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kzv.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnt.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ero.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://trd.yvedp.cn

Go:   // 手写循环
来源：http://dqk.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aiq.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kqb.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://vdk.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hjo.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pwx.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flr.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qao.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pud.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gue.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ezc.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jac.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://gnh.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kaz.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xhh.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftg.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mrn.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzj.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cqt.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfa.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xgk.xziqi.cn

[D26] 数组转字符串
来源：http://ppu.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://chd.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://ynd.meibo888.top

JS:   arr.join(", ")
来源：http://jpy.9152youxi.cn

TS:   arr.join(", ")
来源：http://cid.yuanzhike.top

Java: String.join(", ", list)
来源：http://vsr.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://ygc.bjfxy.top

Ruby: arr.join(", ")
来源：http://uuj.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://kdj.meibo888.top

================================================================================
来源：http://mry.chenlongwang.top

E. 字符串处理
来源：http://bws.havefunace.top

================================================================================
来源：http://ovv.havefunace.top

[E01] 拼接字符串
来源：http://ixq.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rwz.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byf.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pai.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxk.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nso.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mqe.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ytv.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfe.hfpthk.cn

[E02] 重复字符串
来源：http://gmr.316326.xyz

Py:   "ab" * 3
来源：http://wbj.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://srn.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://vgf.yuxming.cn

TS:   "ab".repeat(3)
来源：http://fua.uphjek.com

Java: "ab".repeat(3)
来源：http://rnc.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://jgq.cucudq.cn

Ruby: "ab" * 3
来源：http://das.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sev.jinqigufen.top

[E03] 截取子串
来源：http://qrg.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ndv.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zvc.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eej.cashguo.top

TS:   s.slice(1, 4)
来源：http://itk.nwbrower.top

Java: s.substring(1, 4)
来源：http://zqj.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sbd.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://snp.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://bss.sweek.top

[E04] 查找子串位置
来源：http://rnb.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://vtx.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://ipl.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jvn.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://njx.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://gel.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://hqm.yj20258888.top

Ruby: s.index("x")
来源：http://ytz.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://ncu.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tjc.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gqc.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjy.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oyc.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hnz.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcz.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jzn.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ywn.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ude.bjfxy.top

[E06] 替换子串
来源：http://ysc.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swa.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://uds.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujh.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://cfe.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qie.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hyn.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kbm.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://yri.vehdjk.com

[E07] 按分隔符拆分
来源：http://pjg.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wwn.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kgd.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lse.ppjwa.cn

TS:   s.split(",")
来源：http://tba.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://otg.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://koq.meibo888.top

Ruby: s.split(",");  s.split
来源：http://khi.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nbl.yj202588.top

[E08] 数组按分隔符合并
来源：http://plt.gaohongyu789.top

Py:   ",".join(items)
来源：http://ftn.yj202588.top

PHP:  implode(",", $items);
来源：http://cit.xinyue.icu

JS:   items.join(",")
来源：http://koy.hongshengwenyu.top

TS:   items.join(",")
来源：http://qmp.xuetiantiany.cn

Java: String.join(",", items)
来源：http://unq.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://jaf.xuetiantiany.cn

Ruby: items.join(",")
来源：http://ghf.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://nqp.yuanzhike.top

[E09] 去除所有空白字符
来源：http://egn.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ivt.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xif.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://rxz.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://rmo.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://fxk.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kct.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://dan.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wpe.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://eto.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rjm.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ava.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://ysi.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://hea.vehdjk.com

Java: String.format("%03d", 7)
来源：http://gcu.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://alp.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wtf.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ytv.zhengqikj.top

[E11] 反转字符串
来源：http://vgj.vqdsnc.cn

Py:   s[::-1]
来源：http://dpl.wangdashe.top

PHP:  strrev($s);
来源：http://awv.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://qit.yj20258.top

TS:   [...s].reverse().join("")
来源：http://plg.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ymk.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://scc.bjfxy.top

Ruby: s.reverse
来源：http://bkz.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://guk.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://zbk.fanxiaobao.xyz

Py:   s.count("a")
来源：http://cjd.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://ezh.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://hfy.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://ast.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vvb.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://cic.jlsjyb.cn

Ruby: s.count("a")
来源：http://xwv.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://nff.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://yjo.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://wyh.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qyh.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mvn.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fqh.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tcs.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://inw.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://moq.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zcw.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://usp.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wop.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fim.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rdg.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gmj.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://smn.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mci.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://arq.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gcy.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://zsr.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qfh.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://esa.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lcq.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hvw.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pma.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fgt.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wks.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://myi.bbcook.cn

[E16] 数字千分位
来源：http://hsp.tanke756.top

Py:   f"{1234567:,}"
来源：http://lsb.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://mjj.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wfv.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vmv.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrk.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vet.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spw.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://dmg.hesvh.cn

[E17] 首字母大写
来源：http://rdq.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://grt.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xmz.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qiu.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkt.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ttn.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rlt.jlsjyb.cn

Ruby: s.capitalize
来源：http://qav.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdn.jqgfzy.top

[E18] 模板占位符替换
来源：http://gii.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://stb.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gxi.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mqq.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gpd.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdu.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xpa.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cgm.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mes.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://evs.ydzc1.top

Py:   s.splitlines()
来源：http://ose.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qvb.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://yly.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://dsl.fehbvm.com

Java: s.lines().toList()
来源：http://qfq.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://nbo.zhaomingkeji.xyz

Ruby: s.lines
来源：http://jeq.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://kpy.andypj.xyz

[E20] 判断字符串是否为空
来源：http://kjh.yanxiufei.cn

Py:   if not s:
来源：http://nar.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ncm.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jzl.shuidangran.top

TS:   if (s === "") {}
来源：http://osy.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://qcu.nanxinkj.top


<!-- 参考信息 -->