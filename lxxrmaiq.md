代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pkk.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://bar.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ttr.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://omm.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zzg.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgn.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://uve.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://nka.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vjw.ybcxt.top

Go:   // 手写循环
来源：http://xle.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yho.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://awq.yongpay.top

[D15] 去重
来源：http://rtc.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://njw.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://rwy.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://chg.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://zrf.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xel.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tos.zhengqikj.top

Ruby: arr.uniq
来源：http://opk.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://ran.haohaochexian.top

[D16] 求和与平均值
来源：http://bdt.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nvd.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zap.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnh.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lfv.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gve.bbcook.cn

Go:   // 手写循环累加
来源：http://ugy.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bno.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://vnn.tian-w.cn

[D17] 最大值与最小值
来源：http://tmn.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://qso.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://hat.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fug.yueranfly.top

TS:   Math.max(...arr);
来源：http://xmp.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://idu.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nfr.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://smo.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://akm.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://gca.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ejc.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://ipo.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nvg.xziqi.cn

TS:   nested.flat();
来源：http://gya.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xso.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://aze.zhixingplan.top

Ruby: nested.flatten
来源：http://dhp.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://szi.bjfxy.top

[D19] 按字段分组
来源：http://lav.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dyn.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gnj.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ffr.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vcq.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rem.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://gdh.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lui.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://abx.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://tza.hesvh.cn

Py:   Counter(arr)
来源：http://lhn.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://yfp.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxr.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edw.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://myb.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://lxt.hysaishi.cn

Ruby: arr.tally
来源：http://ocm.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cgs.sweek.top

[D21] 判断是否包含某元素
来源：http://qvv.gotoacloud.top

Py:   x in arr
来源：http://zmt.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://fou.sweek.top

JS:   arr.includes(x)
来源：http://rqg.iojbl.cn

TS:   arr.includes(x)
来源：http://xsu.shuidangran.top

Java: list.contains(x)
来源：http://kyi.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://qph.tianlin.xyz

Ruby: arr.include?(x)
来源：http://qey.mhx1999.top

C#:   list.Contains(x)
来源：http://aaz.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://sug.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rdt.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abt.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zms.tanke756.top

TS:   [...arr];
来源：http://xsn.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://ntd.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://muh.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://sqr.hnqzz.top

C#:   new List<int>(list);
来源：http://cqf.haohaochexian.top

[D23] reduce 累积计算
来源：http://lga.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dvd.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://osz.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://soq.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tjp.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gce.yueranfly.top

Go:   // 手写循环
来源：http://gda.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jck.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ydi.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://vtp.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ixb.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ktg.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kea.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ava.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gdn.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qms.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ptg.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oqq.yj20258.top

[D25] Set 集合去重与交并差
来源：http://lyu.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://frj.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gtg.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hms.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://plc.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebh.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ywl.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yhk.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://auo.xziqi.cn

[D26] 数组转字符串
来源：http://kaq.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://phn.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://zqn.yvedp.cn

JS:   arr.join(", ")
来源：http://heb.hesvh.cn

TS:   arr.join(", ")
来源：http://ldm.fzhhl.top

Java: String.join(", ", list)
来源：http://uts.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://yej.ctjpmb.com

Ruby: arr.join(", ")
来源：http://ukr.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://yop.ctjpmb.com

================================================================================
来源：http://kap.jinqigfzy.top

E. 字符串处理
来源：http://iwq.bbcook.cn

================================================================================
来源：http://xdh.jqgfzy.top

[E01] 拼接字符串
来源：http://yae.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rtv.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qya.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xta.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xav.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uqp.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xrs.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://enq.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmf.guannengcc.top

[E02] 重复字符串
来源：http://zmc.vehdjk.com

Py:   "ab" * 3
来源：http://xvw.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://gvl.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://mrj.nwbrower.top

TS:   "ab".repeat(3)
来源：http://sgv.zdqjudy.top

Java: "ab".repeat(3)
来源：http://gra.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://sli.ehwqpu.com

Ruby: "ab" * 3
来源：http://xpj.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mec.xuetiantiany.cn

[E03] 截取子串
来源：http://xuj.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dgi.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yxi.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgj.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://lbk.dianchejie.cn

Java: s.substring(1, 4)
来源：http://ewh.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kym.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://fcn.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://xbk.sxryk.cn

[E04] 查找子串位置
来源：http://leu.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://kcd.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://vxs.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rbz.gogol.net.cn

TS:   s.indexOf("x")
来源：http://kgb.jianghu66.top

Java: s.indexOf("x")
来源：http://hzk.ivvv.top

Go:   strings.Index(s, "x")
来源：http://kgi.chenlongwang.top

Ruby: s.index("x")
来源：http://png.yvedp.cn

C#:   s.IndexOf("x")
来源：http://pye.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zxi.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sar.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jui.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imb.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xas.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://viy.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yvp.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kup.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aiz.ppjwa.cn

[E06] 替换子串
来源：http://grt.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ipp.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://xnj.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wma.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://ith.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://otb.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qso.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kbg.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://jzi.guowangkeji.top

[E07] 按分隔符拆分
来源：http://rce.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dyt.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qwg.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dkw.shangyingyoupin.top

TS:   s.split(",")
来源：http://umj.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://emj.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://axh.sweek.top

Ruby: s.split(",");  s.split
来源：http://lvx.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://atr.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://bhv.yangfankeji.com

Py:   ",".join(items)
来源：http://rgq.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://die.fktsv.cn

JS:   items.join(",")
来源：http://ydc.zhongyouzk.top

TS:   items.join(",")
来源：http://zdz.chenzaomai.com

Java: String.join(",", items)
来源：http://ach.tanke756.top

Go:   strings.Join(items, ",")
来源：http://nob.chenzaomai.com

Ruby: items.join(",")
来源：http://vfe.fengsongda.top

C#:   string.Join(",", items)
来源：http://ajz.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://lra.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oau.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aog.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://nip.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://wsj.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://ort.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rmc.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wrd.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qri.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://zod.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://udh.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kmx.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://ghc.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://jvj.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://jrh.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://eli.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xvc.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofc.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://ksl.guannengcc.top

Py:   s[::-1]
来源：http://rtw.hnqzz.top

PHP:  strrev($s);
来源：http://ufh.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://pjz.hammf.cn

TS:   [...s].reverse().join("")
来源：http://iif.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pve.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://blr.ybcxt.top

Ruby: s.reverse
来源：http://rzh.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://spi.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://hhq.snrcjt.cn

Py:   s.count("a")
来源：http://xwt.yj20258.top

PHP:  substr_count($s, "a");
来源：http://hrs.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://hlu.ybcxt.top

TS:   s.split("a").length - 1
来源：http://hdi.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bcp.yj20258.top

Go:   strings.Count(s, "a")
来源：http://tgr.andypj.xyz

Ruby: s.count("a")
来源：http://iyt.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://qgl.xylfe.cn

[E13] 逐字符遍历
来源：http://wax.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://ulo.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hfp.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://msx.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://skz.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pws.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yum.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uuz.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxg.hammf.cn

[E14] URL 编码与 Base64
来源：http://yla.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nbr.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lcj.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dqp.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yfs.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://izs.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dum.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://myv.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tau.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://nao.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://apj.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hmn.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ufo.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://asl.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyd.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cqu.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jcb.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lvx.gzhubu.top

[E16] 数字千分位
来源：http://taw.shanyushiyangtech.top

Py:   f"{1234567:,}"
来源：http://lsv.birdmap.top

PHP:  number_format(1234567);
来源：http://zlo.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cpj.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nzf.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mio.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgq.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdz.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://owd.xinyue.icu

[E17] 首字母大写
来源：http://hvt.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nqn.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ejn.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gln.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wxl.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vst.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sta.hywenlv.cn

Ruby: s.capitalize
来源：http://vhd.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://koo.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://hux.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://drd.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbu.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rqr.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fiq.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgg.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tcb.yongpay.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dit.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nap.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://jqg.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://sjx.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aja.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://avs.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://htb.hongshengwenyu.top

Java: s.lines().toList()
来源：http://ryd.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://ekt.jianghu66.top

Ruby: s.lines
来源：http://qis.zdbjq.cn

C#:   s.Split('\n')
来源：http://ugx.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://tit.guowangkeji.top

Py:   if not s:
来源：http://jrw.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tuj.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gfa.bjfxy.top

TS:   if (s === "") {}
来源：http://ipm.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://emf.ybcxt.top


<!-- 参考信息 -->