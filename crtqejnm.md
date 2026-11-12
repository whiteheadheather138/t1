代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mbk.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qid.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://owf.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://nvn.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfu.bbcook.cn

Go:   // 手写循环
来源：http://mzh.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://bxd.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ptw.yongpay.top

[D15] 去重
来源：http://ytk.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://stb.nwbrower.top

PHP:  array_unique($arr);
来源：http://gwv.daxiang520.top

JS:   [...new Set(arr)]
来源：http://nyj.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://xca.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gft.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sfk.zhiwuduotai.top

Ruby: arr.uniq
来源：http://xlm.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://nsh.redwolf501.top

[D16] 求和与平均值
来源：http://oxi.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://njo.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vvr.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://llr.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tbk.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zrw.haohaochexian.top

Go:   // 手写循环累加
来源：http://soc.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eaa.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://phg.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://icy.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://soz.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://lfr.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://alb.epnwcf.com

TS:   Math.max(...arr);
来源：http://jsy.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jcs.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vet.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://gmm.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://ymy.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://oep.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jkd.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://zfv.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zoj.hnxiangtu.top

TS:   nested.flat();
来源：http://ncb.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ovt.nanxinkj.top

Go:   // 手写双层循环
来源：http://gsk.sysykeji.top

Ruby: nested.flatten
来源：http://ncq.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dkn.ydjk.org.cn

[D19] 按字段分组
来源：http://gan.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qbb.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xfr.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bhw.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://dws.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jqb.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://tqf.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ejw.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fcd.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://eis.meibo888.top

Py:   Counter(arr)
来源：http://skc.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://ova.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iru.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rct.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mxp.yj202588.top

Go:   // 手写 map[T]int
来源：http://ubb.tianlin.xyz

Ruby: arr.tally
来源：http://hnp.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://amg.yvedp.cn

[D21] 判断是否包含某元素
来源：http://mvy.316326.xyz

Py:   x in arr
来源：http://oyx.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://xoy.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://stt.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://aji.uphjek.com

Java: list.contains(x)
来源：http://fmj.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://hxx.yueranfly.top

Ruby: arr.include?(x)
来源：http://ikg.hcnkem.com

C#:   list.Contains(x)
来源：http://jqu.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://xwh.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nki.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gaj.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hof.zhijiandao.cn

TS:   [...arr];
来源：http://fyw.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://ksc.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://bum.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://gpr.jinqigfzy.top

C#:   new List<int>(list);
来源：http://olq.nwbrower.top

[D23] reduce 累积计算
来源：http://ltw.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ecc.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzm.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fuh.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bkn.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fod.ydjk.org.cn

Go:   // 手写循环
来源：http://xgy.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yjp.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gck.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://umk.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qlq.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wzf.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://frb.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fuk.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fls.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xdx.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mhr.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zyf.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://pdf.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://igs.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyp.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lox.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://daj.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wte.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lsd.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://poy.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://urq.wangdashe.top

[D26] 数组转字符串
来源：http://zkn.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://vrs.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://tzw.yueranfly.top

JS:   arr.join(", ")
来源：http://xva.yongpay.top

TS:   arr.join(", ")
来源：http://fnc.meibo888.top

Java: String.join(", ", list)
来源：http://obt.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://zyu.xinyue.icu

Ruby: arr.join(", ")
来源：http://xxh.0kj1m.cn

C#:   string.Join(", ", list)
来源：http://xhp.9152youxi.cn

================================================================================
来源：http://anw.meibo888.top

E. 字符串处理
来源：http://xys.xingfuxueyuan.xyz

================================================================================
来源：http://vhw.bbcook.cn

[E01] 拼接字符串
来源：http://zil.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jgm.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mhs.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dnf.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mag.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mdr.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://txy.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pgn.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gtw.fktsv.cn

[E02] 重复字符串
来源：http://aih.0kj1m.cn

Py:   "ab" * 3
来源：http://zcd.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://qzp.mhx1999.top

JS:   "ab".repeat(3)
来源：http://qgo.guannengcc.top

TS:   "ab".repeat(3)
来源：http://fhl.cashguo.top

Java: "ab".repeat(3)
来源：http://xex.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://frj.gaohongyu789.top

Ruby: "ab" * 3
来源：http://nlu.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wnb.yfazqb.com

[E03] 截取子串
来源：http://mgh.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pvm.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lsx.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xdu.hnqzz.top

TS:   s.slice(1, 4)
来源：http://mbe.hammf.cn

Java: s.substring(1, 4)
来源：http://mbz.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nmt.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://max.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://xgi.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://pkt.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://qup.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://riv.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ops.hfpthk.cn

TS:   s.indexOf("x")
来源：http://zyi.ivvv.top

Java: s.indexOf("x")
来源：http://yne.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://pig.fzhhl.top

Ruby: s.index("x")
来源：http://ijs.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://aij.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://pks.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ilu.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vou.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ono.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dra.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yql.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ypk.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kxm.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uww.wangshuangyany.cn

[E06] 替换子串
来源：http://sxz.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vbt.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://laf.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dtg.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://cnq.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ybl.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bab.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wua.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://mwm.pycfn.com

[E07] 按分隔符拆分
来源：http://kry.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jke.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pqc.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wak.tian-w.cn

TS:   s.split(",")
来源：http://yxp.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://fnd.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ldt.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://mxf.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ssw.birdmap.top

[E08] 数组按分隔符合并
来源：http://umn.hesvh.cn

Py:   ",".join(items)
来源：http://yzg.cdnleiting.top

PHP:  implode(",", $items);
来源：http://hiy.yuxming.cn

JS:   items.join(",")
来源：http://tfk.fehbvm.com

TS:   items.join(",")
来源：http://tgl.tanke756.top

Java: String.join(",", items)
来源：http://pvj.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://qfv.sjlbkw.cn

Ruby: items.join(",")
来源：http://ufy.sweek.top

C#:   string.Join(",", items)
来源：http://kho.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://zzf.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lzf.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://joj.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://edg.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://naq.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://gix.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://twg.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://heu.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cut.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://kvg.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xri.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bcg.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://bhp.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://mmj.nwbrower.top

Java: String.format("%03d", 7)
来源：http://npp.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cyr.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mqn.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zei.nanxinkj.top

[E11] 反转字符串
来源：http://mtf.cashguo.top

Py:   s[::-1]
来源：http://oln.zhengqikj.top

PHP:  strrev($s);
来源：http://wqg.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://mnw.havefunace.top

TS:   [...s].reverse().join("")
来源：http://kwo.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://gov.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://qms.meibo888.top

Ruby: s.reverse
来源：http://qzb.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://mcz.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://rjf.vqdsnc.cn

Py:   s.count("a")
来源：http://gio.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://smc.hesvh.cn

JS:   s.split("a").length - 1
来源：http://jwu.316326.xyz

TS:   s.split("a").length - 1
来源：http://atm.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eva.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://dkv.tianlin.xyz

Ruby: s.count("a")
来源：http://mjt.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://lww.tianlin.xyz

[E13] 逐字符遍历
来源：http://tbv.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://zbr.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zzx.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bbs.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rxq.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ueb.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yyy.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ddr.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jwl.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://xhm.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oki.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://umg.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ugy.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ffe.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jwo.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://emn.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://irp.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cyw.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://rlf.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hbj.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vle.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ury.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sdi.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dnp.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xxh.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbf.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://stv.uphjek.com

[E16] 数字千分位
来源：http://dhl.hnqzz.top

Py:   f"{1234567:,}"
来源：http://mco.cdnleiting.top

PHP:  number_format(1234567);
来源：http://vvt.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://wtv.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://krr.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qzc.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kdq.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rwl.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://ekp.wangshuangyany.cn

[E17] 首字母大写
来源：http://bdw.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nmr.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ccq.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kiv.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cie.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cra.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wqk.epnwcf.com

Ruby: s.capitalize
来源：http://opz.haohaochexian.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://llz.aibaodan.cn

[E18] 模板占位符替换
来源：http://qjs.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gvs.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jsn.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kar.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rrs.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nqo.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yco.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hud.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrt.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://jch.nanxuanxn.top

Py:   s.splitlines()
来源：http://dvz.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dyx.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://awj.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://cbc.cqqwz.cn

Java: s.lines().toList()
来源：http://sad.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://osq.dashuyun.cn

Ruby: s.lines
来源：http://bim.zhijiandao.cn

C#:   s.Split('\n')
来源：http://uak.hnqzz.top

[E20] 判断字符串是否为空
来源：http://wjq.shuidangran.top

Py:   if not s:
来源：http://uty.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hxf.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jvy.fengsongda.top

TS:   if (s === "") {}
来源：http://hnu.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://mya.shzxlz.cn

Go:   if s == "" {}
来源：http://jgw.hammf.cn

Ruby: if s.empty?
来源：http://nbl.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ing.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://xnw.quarkkingdee.top


<!-- 参考信息 -->