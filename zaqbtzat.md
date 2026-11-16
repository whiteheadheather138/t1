代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qjx.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://arv.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://xhh.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lng.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gyf.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hla.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gjj.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://pwa.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://efi.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qnk.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://ify.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://udt.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xdm.haohaochexian.top

Go:   // 手写循环
来源：http://qmt.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://svw.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gmg.hysaishi.cn

[D15] 去重
来源：http://woa.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dqy.yfazqb.com

PHP:  array_unique($arr);
来源：http://jzs.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://vrk.yongpay.top

TS:   [...new Set(arr)]
来源：http://ojq.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://byw.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://zfx.316326.xyz

Ruby: arr.uniq
来源：http://aey.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://oio.jianghu66.top

[D16] 求和与平均值
来源：http://kwf.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hws.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bpa.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://osa.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qvw.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mdo.jlsjyb.cn

Go:   // 手写循环累加
来源：http://vpk.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qvx.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://cir.52xcode.cn

[D17] 最大值与最小值
来源：http://wxk.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://hjk.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://rys.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dwc.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://xgv.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nbq.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lua.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://asr.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://ome.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://wsj.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oyl.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://pjc.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nlo.sweek.top

TS:   nested.flat();
来源：http://tea.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dub.jyoumei.cn

Go:   // 手写双层循环
来源：http://iwr.cqqwz.cn

Ruby: nested.flatten
来源：http://mqh.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mgu.jiagoushi.top

[D19] 按字段分组
来源：http://iyl.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://usf.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xbd.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgk.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://bfa.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iol.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://zst.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uhi.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fgz.hammf.cn

[D20] 统计每个元素出现次数
来源：http://ogr.hesvh.cn

Py:   Counter(arr)
来源：http://nfq.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://byx.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxg.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ugg.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lpb.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://fis.bjfxy.top

Ruby: arr.tally
来源：http://whv.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uhv.fzhhl.top

[D21] 判断是否包含某元素
来源：http://dti.sysykeji.top

Py:   x in arr
来源：http://wvv.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://vfl.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://akf.fktsv.cn

TS:   arr.includes(x)
来源：http://fho.mhx1999.top

Java: list.contains(x)
来源：http://kry.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://dxq.ppjwa.cn

Ruby: arr.include?(x)
来源：http://tuz.zhijiandao.cn

C#:   list.Contains(x)
来源：http://zav.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://syk.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://esb.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zoy.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oet.nanxuanxn.top

TS:   [...arr];
来源：http://dwx.fengsongda.top

Java: new ArrayList<>(list);
来源：http://ige.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://veo.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://zpq.0kj1m.cn

C#:   new List<int>(list);
来源：http://fgv.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://oky.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bmt.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqp.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmb.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhz.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfz.sufxvd.cn

Go:   // 手写循环
来源：http://swx.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yvq.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://glo.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://awn.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lam.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rej.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://prr.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jxd.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bsp.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qzk.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yvg.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyk.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://ita.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hch.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://llj.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pyv.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mkq.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oew.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://csd.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vmi.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsg.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://ncg.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://fpj.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://zvx.sjlbkw.cn

JS:   arr.join(", ")
来源：http://gyt.nwbrower.top

TS:   arr.join(", ")
来源：http://dgl.birdmap.top

Java: String.join(", ", list)
来源：http://pqy.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://mck.pycfn.com

Ruby: arr.join(", ")
来源：http://toz.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://yoi.vehdjk.com

================================================================================
来源：http://peg.chenzaomai.com

E. 字符串处理
来源：http://nhb.hongshengwenyu.top

================================================================================
来源：http://zaw.fengsongda.top

[E01] 拼接字符串
来源：http://pzh.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kqe.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://opm.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tak.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyp.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tju.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aub.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sup.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ynz.ydzc1.top

[E02] 重复字符串
来源：http://aqf.snrcjt.cn

Py:   "ab" * 3
来源：http://ffd.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://ekt.yvedp.cn

JS:   "ab".repeat(3)
来源：http://tnf.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://xap.fehbvm.com

Java: "ab".repeat(3)
来源：http://gkp.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://ypu.xylfe.cn

Ruby: "ab" * 3
来源：http://cxw.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pwe.shanyushiyangtech.top

[E03] 截取子串
来源：http://xct.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hdh.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjb.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://grj.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://hcs.pycfn.com

Java: s.substring(1, 4)
来源：http://goq.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fvx.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://gak.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://vae.jinqigufen.top

[E04] 查找子串位置
来源：http://rsl.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://wov.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://ghu.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kce.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://cwy.sufxvd.cn

Java: s.indexOf("x")
来源：http://agt.meibo888.top

Go:   strings.Index(s, "x")
来源：http://dta.dashuyun.cn

Ruby: s.index("x")
来源：http://ryf.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://vfs.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cfl.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zmu.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hbj.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ash.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cwp.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yns.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sha.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kcc.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qeu.hysaishi.cn

[E06] 替换子串
来源：http://tus.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rgc.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://hlx.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wns.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://igm.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psg.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ifj.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kkj.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://yry.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://ifs.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ouq.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybd.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ngt.xuanzx.com

TS:   s.split(",")
来源：http://qor.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://rbo.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://udc.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://wyn.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://krj.c1oappe.top

[E08] 数组按分隔符合并
来源：http://cbz.ctjpmb.com

Py:   ",".join(items)
来源：http://tzk.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://ccd.pengpengdd.cyou

JS:   items.join(",")
来源：http://ett.fzhhl.top

TS:   items.join(",")
来源：http://wwp.hcnkem.com

Java: String.join(",", items)
来源：http://pvg.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://zca.wangdashe.top

Ruby: items.join(",")
来源：http://kei.haohaochexian.top

C#:   string.Join(",", items)
来源：http://lrk.jianghu66.top

[E09] 去除所有空白字符
来源：http://erj.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ggc.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pwt.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://vay.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://sjx.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://iae.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://evi.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wqc.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xgv.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://hyg.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hck.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gmh.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://fbf.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://fqb.tanke756.top

Java: String.format("%03d", 7)
来源：http://apn.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://udv.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yki.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oah.hywenlv.cn

[E11] 反转字符串
来源：http://tfd.hnxiangtu.top

Py:   s[::-1]
来源：http://gps.iojbl.cn

PHP:  strrev($s);
来源：http://iiz.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://sro.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://syt.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lud.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yav.ivvv.top

Ruby: s.reverse
来源：http://jrt.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://yex.52xcode.cn

[E12] 统计某字符出现次数
来源：http://hna.bbcook.cn

Py:   s.count("a")
来源：http://osi.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://uhi.hammf.cn

JS:   s.split("a").length - 1
来源：http://gij.smart0.xyz

TS:   s.split("a").length - 1
来源：http://dbh.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hol.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://fsx.snrcjt.cn

Ruby: s.count("a")
来源：http://lhc.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://tsn.gzhubu.top

[E13] 逐字符遍历
来源：http://ixm.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://ngt.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://git.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qqh.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qal.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dvo.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mlc.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bmf.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eky.52xcode.cn

[E14] URL 编码与 Base64
来源：http://ndl.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tbx.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yis.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ybo.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wab.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://run.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vat.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uih.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nxr.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://fkq.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ugc.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sck.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zsn.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ndg.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cpr.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://txv.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://knz.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cnz.aibaodan.cn

[E16] 数字千分位
来源：http://hze.tarul.cn

Py:   f"{1234567:,}"
来源：http://evz.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://gph.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ybe.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jsn.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxa.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jmg.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fhd.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://dnv.ehwqpu.com

[E17] 首字母大写
来源：http://frl.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ynz.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldc.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qgx.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvo.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oju.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iis.xuanzx.com

Ruby: s.capitalize
来源：http://wvc.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://stk.snrcjt.cn

[E18] 模板占位符替换
来源：http://bmk.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xzq.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://crt.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://duu.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fgt.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lvc.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pvd.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kka.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://izs.cucudq.cn

[E19] 多行文本按行拆分
来源：http://ojq.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://rag.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kvz.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://cmv.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://yxj.jqgufenzy.top

Java: s.lines().toList()
来源：http://fxi.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://vnb.52xcode.cn

Ruby: s.lines
来源：http://dle.daxiang520.top

C#:   s.Split('\n')
来源：http://hoy.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://kos.ydzc1.top

Py:   if not s:
来源：http://abl.guannengcc.top


<!-- 参考信息 -->