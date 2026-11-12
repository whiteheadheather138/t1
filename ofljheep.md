代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dbl.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ghm.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://acd.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://xbh.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ren.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ges.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://htr.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://oyw.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eok.shzxlz.cn

Go:   // 手写循环
来源：http://uwz.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://ffu.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pfq.vqdsnc.cn

[D15] 去重
来源：http://rev.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fxe.bjfxy.top

PHP:  array_unique($arr);
来源：http://bov.fengsongda.top

JS:   [...new Set(arr)]
来源：http://poe.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://lil.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fcu.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://nme.0kj1m.cn

Ruby: arr.uniq
来源：http://nnj.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://zpl.ydzc1.top

[D16] 求和与平均值
来源：http://dtv.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hcs.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lsz.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iaa.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cmw.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kwf.yonumen.top

Go:   // 手写循环累加
来源：http://ikf.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aag.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://xmg.daxiang520.top

[D17] 最大值与最小值
来源：http://irb.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://xgd.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://rja.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mdu.dashuyun.cn

TS:   Math.max(...arr);
来源：http://koq.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://del.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nxj.yonumen.top

Ruby: arr.max;  arr.min
来源：http://qyp.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://txw.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://fnr.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://its.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://ydl.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ipl.uphjek.com

TS:   nested.flat();
来源：http://gly.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pkn.52xcode.cn

Go:   // 手写双层循环
来源：http://tlf.wangshuangyany.cn

Ruby: nested.flatten
来源：http://jog.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://klc.gzhubu.top

[D19] 按字段分组
来源：http://nxr.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xqe.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hyg.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mbg.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://jxq.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ony.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://svb.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eho.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ehc.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://tnv.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://zwc.fehbvm.com

PHP:  array_count_values($arr);
来源：http://hag.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://orm.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://soa.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://com.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://ypm.jinqigfzy.top

Ruby: arr.tally
来源：http://fqp.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sfn.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://nxo.yvedp.cn

Py:   x in arr
来源：http://fpc.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://not.iojbl.cn

JS:   arr.includes(x)
来源：http://cpv.ctjpmb.com

TS:   arr.includes(x)
来源：http://zty.hywenlv.cn

Java: list.contains(x)
来源：http://tob.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://sxg.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://nrv.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://yri.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://usf.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wxu.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ndy.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wov.9152youxi.cn

TS:   [...arr];
来源：http://ohi.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://vnc.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xma.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://auw.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://wra.gaohongyu789.top

[D23] reduce 累积计算
来源：http://qzr.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sun.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gtj.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ypk.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdq.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tle.sufxvd.cn

Go:   // 手写循环
来源：http://ktq.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jja.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dgt.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://lcl.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pxh.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://keu.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://njz.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oii.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ept.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewt.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rki.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://arv.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://fkz.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://clm.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hcc.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bcp.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yxj.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xgx.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bxl.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwy.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ebw.yueranfly.top

[D26] 数组转字符串
来源：http://odq.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://tps.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://fzp.dianchejie.cn

JS:   arr.join(", ")
来源：http://wal.nanxinkj.top

TS:   arr.join(", ")
来源：http://lji.jqgufenzy.top

Java: String.join(", ", list)
来源：http://ucv.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://rrj.zhengqikj.top

Ruby: arr.join(", ")
来源：http://isw.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://iad.redwolf501.top

================================================================================
来源：http://tpf.hfpthk.cn

E. 字符串处理
来源：http://eim.sysykeji.top

================================================================================
来源：http://sbo.mhx1999.top

[E01] 拼接字符串
来源：http://cix.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xle.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hil.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kii.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://osz.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cwm.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gyn.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zxx.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://snu.vqdsnc.cn

[E02] 重复字符串
来源：http://qjs.yongpay.top

Py:   "ab" * 3
来源：http://wsq.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://dkr.hesvh.cn

JS:   "ab".repeat(3)
来源：http://kwx.xylfe.cn

TS:   "ab".repeat(3)
来源：http://msp.yfazqb.com

Java: "ab".repeat(3)
来源：http://cif.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://sag.haohaochexian.top

Ruby: "ab" * 3
来源：http://pxe.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wpm.pycfn.com

[E03] 截取子串
来源：http://cfp.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uxs.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://llu.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://skb.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://gks.yj20258.top

Java: s.substring(1, 4)
来源：http://snp.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rpn.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://yzw.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://jsb.smart0.xyz

[E04] 查找子串位置
来源：http://iob.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://eis.daria6918.cn

PHP:  strpos($s, "x");
来源：http://zpq.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gwu.daxiang520.top

TS:   s.indexOf("x")
来源：http://xij.hfpthk.cn

Java: s.indexOf("x")
来源：http://xen.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://zpj.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://cip.jianghu66.top

C#:   s.IndexOf("x")
来源：http://rnz.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lzh.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iic.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rpb.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnf.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://exl.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edu.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qwq.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fee.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fcb.tanke756.top

[E06] 替换子串
来源：http://fql.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gyg.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://gpg.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbj.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://gsq.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idb.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://odj.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ogr.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://xbm.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://uvc.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwj.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcy.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://csv.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://tut.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ezd.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymo.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://nrf.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esp.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://cyn.yueranfly.top

Py:   ",".join(items)
来源：http://omx.zycfv.cn

PHP:  implode(",", $items);
来源：http://noz.shanyushiyangtech.top

JS:   items.join(",")
来源：http://mxh.feifeiyinyue.top

TS:   items.join(",")
来源：http://oos.jqgfzy.top

Java: String.join(",", items)
来源：http://dmr.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://shk.fktsv.cn

Ruby: items.join(",")
来源：http://iad.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://ruf.jyoumei.cn

[E09] 去除所有空白字符
来源：http://onz.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vqq.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lsm.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://kpo.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://ksu.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ixq.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdh.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://gso.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://orn.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://dxt.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eou.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dan.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://ylv.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://qho.redwolf501.top

Java: String.format("%03d", 7)
来源：http://mbw.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tse.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ldi.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xtw.guannengcc.top

[E11] 反转字符串
来源：http://ifc.0kj1m.cn

Py:   s[::-1]
来源：http://isx.ctjpmb.com

PHP:  strrev($s);
来源：http://oik.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://oxh.hammf.cn

TS:   [...s].reverse().join("")
来源：http://yxn.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://jth.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://klr.tarul.cn

Ruby: s.reverse
来源：http://ktw.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bvi.andypj.xyz

[E12] 统计某字符出现次数
来源：http://fao.daria6918.cn

Py:   s.count("a")
来源：http://nic.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://hya.hammf.cn

JS:   s.split("a").length - 1
来源：http://skd.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://jmi.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zne.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://pwm.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://ujr.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://vdh.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://yvl.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://apv.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rqj.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yqn.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://haw.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lud.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://drw.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://azm.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fnz.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://lms.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nvt.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://dgv.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://arp.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qsb.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owp.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://emz.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ogc.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jci.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://uak.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://psn.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wek.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fsl.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qio.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kjb.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jfv.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gym.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://avc.smart0.xyz

[E16] 数字千分位
来源：http://ioc.gzhubu.top

Py:   f"{1234567:,}"
来源：http://ayg.nanxinkj.top

PHP:  number_format(1234567);
来源：http://uvz.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gaj.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rbq.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hnq.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bxz.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yhf.tanke756.top

C#:   1234567.ToString("N0")
来源：http://row.jinqigfzy.top

[E17] 首字母大写
来源：http://cqm.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ihj.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ndi.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsp.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yum.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vso.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yon.jqgufenzy.top

Ruby: s.capitalize
来源：http://igi.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lln.nwbrower.top

[E18] 模板占位符替换
来源：http://fsx.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gek.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bjq.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oks.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gix.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ihd.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rer.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dew.shangyingyoupin.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zdy.sxryk.cn

[E19] 多行文本按行拆分
来源：http://zpx.shzxlz.cn

Py:   s.splitlines()
来源：http://xmz.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oaa.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://mef.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://lxu.yonumen.top

Java: s.lines().toList()
来源：http://vky.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://hjn.zhongyouzk.top

Ruby: s.lines
来源：http://fvv.yonumen.top

C#:   s.Split('\n')
来源：http://hcf.smart0.xyz

[E20] 判断字符串是否为空
来源：http://cfd.xinyue.icu

Py:   if not s:
来源：http://njq.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iju.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kzi.uphjek.com

TS:   if (s === "") {}
来源：http://nvx.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://vww.meibo888.top


<!-- 参考信息 -->