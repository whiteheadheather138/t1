代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zxc.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://oif.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://bha.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uhp.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uic.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://wig.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kvc.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://sfq.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://adu.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://llp.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://ncu.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://xrg.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://waj.kuanghao11.cn

Go:   // 手写循环
来源：http://wzt.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://ztk.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dir.sxryk.cn

[D15] 去重
来源：http://ipy.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dss.tanke756.top

PHP:  array_unique($arr);
来源：http://gtq.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://dpm.jianghu66.top

TS:   [...new Set(arr)]
来源：http://kem.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ljg.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ojr.zhongyouzk.top

Ruby: arr.uniq
来源：http://gar.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://kbp.aizwys.cn

[D16] 求和与平均值
来源：http://cjm.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nny.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cip.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yqp.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://goz.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dbc.sjlbkw.cn

Go:   // 手写循环累加
来源：http://ctb.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yil.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://bgm.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://vym.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://yhk.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://uvx.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yaq.guannengcc.top

TS:   Math.max(...arr);
来源：http://izw.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://csn.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rag.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://jtf.cashguo.top

C#:   list.Max();  list.Min()
来源：http://lck.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://qrn.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uyj.yongpay.top

PHP:  array_merge(...$nested);
来源：http://phj.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kkn.fengsongda.top

TS:   nested.flat();
来源：http://ypo.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ort.hnxiangtu.top

Go:   // 手写双层循环
来源：http://tve.bjfxy.top

Ruby: nested.flatten
来源：http://fjh.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jew.daxiang520.top

[D19] 按字段分组
来源：http://lnu.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tyz.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kqd.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uzz.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vut.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zuj.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://xmt.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mxj.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xva.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://utr.fehbvm.com

Py:   Counter(arr)
来源：http://yyr.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://xlz.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://krw.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hcm.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ckl.yj20258.top

Go:   // 手写 map[T]int
来源：http://xbp.xuetiantiany.cn

Ruby: arr.tally
来源：http://nwh.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://goy.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://dca.dashuyun.cn

Py:   x in arr
来源：http://pan.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://gdn.jlsjyb.cn

JS:   arr.includes(x)
来源：http://xab.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://wrz.jlsjyb.cn

Java: list.contains(x)
来源：http://bsa.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://yww.gzhubu.top

Ruby: arr.include?(x)
来源：http://xsn.redwolf501.top

C#:   list.Contains(x)
来源：http://gwr.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://voo.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zsg.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wai.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hoq.zhiwuduotai.top

TS:   [...arr];
来源：http://ven.yj20258888.top

Java: new ArrayList<>(list);
来源：http://ptu.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://plj.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://ngd.52xcode.cn

C#:   new List<int>(list);
来源：http://ojw.zhongyouzk.top

[D23] reduce 累积计算
来源：http://ury.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dcp.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uhu.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjg.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyi.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ffw.cucudq.cn

Go:   // 手写循环
来源：http://byg.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sau.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://poa.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://rel.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yls.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cvo.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://van.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ntw.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wkm.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ayg.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gwb.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ith.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://tat.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lcr.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pyx.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bfg.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ydj.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yly.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vok.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wrt.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qsj.yj20258888.top

[D26] 数组转字符串
来源：http://mml.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://uft.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://tam.ctjpmb.com

JS:   arr.join(", ")
来源：http://zfn.yuanzhike.top

TS:   arr.join(", ")
来源：http://mre.zycfv.cn

Java: String.join(", ", list)
来源：http://sxn.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://lhu.fengsongda.top

Ruby: arr.join(", ")
来源：http://xos.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://drj.pycfn.com

================================================================================
来源：http://wmn.bbcook.cn

E. 字符串处理
来源：http://bdi.uphjek.com

================================================================================
来源：http://rmf.guannengcc.top

[E01] 拼接字符串
来源：http://qxx.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wnn.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cdw.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eff.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rfp.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://twa.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yxb.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://auk.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ykw.shuidangran.top

[E02] 重复字符串
来源：http://yni.dianchejie.cn

Py:   "ab" * 3
来源：http://lsx.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://lok.andypj.xyz

JS:   "ab".repeat(3)
来源：http://xyv.316326.xyz

TS:   "ab".repeat(3)
来源：http://lkf.chenlongwang.top

Java: "ab".repeat(3)
来源：http://hps.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://vyz.fengsongda.top

Ruby: "ab" * 3
来源：http://ubt.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mgv.smart0.xyz

[E03] 截取子串
来源：http://nng.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyu.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqp.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wgp.bbcook.cn

TS:   s.slice(1, 4)
来源：http://wzx.snrcjt.cn

Java: s.substring(1, 4)
来源：http://hoh.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ykv.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://qld.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://akj.yj202588.top

[E04] 查找子串位置
来源：http://khq.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://lcf.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://cqy.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qhe.sufxvd.cn

TS:   s.indexOf("x")
来源：http://fdi.gogol.net.cn

Java: s.indexOf("x")
来源：http://vgu.sweek.top

Go:   strings.Index(s, "x")
来源：http://xtq.hnqzz.top

Ruby: s.index("x")
来源：http://jof.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://hln.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xiq.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://izq.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://skr.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vox.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mvr.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://huu.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fdb.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vzm.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rsv.nanxuanxn.top

[E06] 替换子串
来源：http://jta.0kj1m.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nhb.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://anl.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://thp.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://hqb.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqg.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://buk.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vzd.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://tie.epnwcf.com

[E07] 按分隔符拆分
来源：http://piy.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sni.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ghl.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vry.quarkkingdee.top

TS:   s.split(",")
来源：http://ler.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://twl.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tib.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://rot.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dsy.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://kfo.zdqjudy.top

Py:   ",".join(items)
来源：http://ant.havefunace.top

PHP:  implode(",", $items);
来源：http://vdc.zdqjudy.top

JS:   items.join(",")
来源：http://dny.yangfankeji.com

TS:   items.join(",")
来源：http://rps.c1oappe.top

Java: String.join(",", items)
来源：http://eed.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://fhi.yuxming.cn

Ruby: items.join(",")
来源：http://urr.52xcode.cn

C#:   string.Join(",", items)
来源：http://rdt.chenlongwang.top

[E09] 去除所有空白字符
来源：http://nyk.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jye.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wdn.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://xsg.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://aty.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://unh.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fqm.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://vqk.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rju.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://jkb.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vjb.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ete.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://dut.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://dms.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://cir.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rzj.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dph.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oyh.tianlin.xyz

[E11] 反转字符串
来源：http://rqd.sweek.top

Py:   s[::-1]
来源：http://pqt.fengsongda.top

PHP:  strrev($s);
来源：http://lbw.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://wui.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://bgo.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://arw.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lal.fehbvm.com

Ruby: s.reverse
来源：http://zqd.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rha.smart0.xyz

[E12] 统计某字符出现次数
来源：http://zks.nanxinkj.top

Py:   s.count("a")
来源：http://akn.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://jrf.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://wtl.guannengcc.top

TS:   s.split("a").length - 1
来源：http://prd.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ddu.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://kfs.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://esd.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://vta.zhongyouzk.top

[E13] 逐字符遍历
来源：http://fdm.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://zma.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yfj.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://juy.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pns.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xyo.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qgd.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://amn.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://czb.fehbvm.com

[E14] URL 编码与 Base64
来源：http://fcu.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ejh.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://scy.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eor.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dym.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hal.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wzc.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hyy.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsv.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://pkk.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ubn.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oxn.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://flc.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uai.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bln.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://syk.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qkb.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ixr.yongpay.top

[E16] 数字千分位
来源：http://otm.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://dpk.ivvv.top

PHP:  number_format(1234567);
来源：http://lvb.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ezv.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dkk.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xrb.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://irn.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ojf.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://vzh.iojbl.cn

[E17] 首字母大写
来源：http://aen.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jsi.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zfx.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nan.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyc.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ivt.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kic.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://pmk.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://isp.epnwcf.com

[E18] 模板占位符替换
来源：http://ilo.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ang.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://irl.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ktu.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tkw.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ove.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wuu.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jwz.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nyi.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://tzm.cashguo.top

Py:   s.splitlines()
来源：http://wpt.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://czw.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://mun.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://djn.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://rhf.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://eua.feifeiyinyue.top

Ruby: s.lines
来源：http://rql.bbcook.cn

C#:   s.Split('\n')
来源：http://scq.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://fxu.hywenlv.cn

Py:   if not s:
来源：http://qcm.fanxiaobao.xyz


<!-- 参考信息 -->