代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pmd.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://aiz.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://zhc.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vqv.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nub.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://owd.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uce.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://max.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://whx.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://occ.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://piu.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://ktt.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nyt.nanxuanxn.top

Go:   // 手写循环
来源：http://lht.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://drb.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ycm.bbcook.cn

[D15] 去重
来源：http://mis.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://din.yangfankeji.com

PHP:  array_unique($arr);
来源：http://okd.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://gxu.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://seb.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://csu.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://vvp.0kj1m.cn

Ruby: arr.uniq
来源：http://nic.birdmap.top

C#:   list.Distinct().ToList()
来源：http://csq.ydzc1.top

[D16] 求和与平均值
来源：http://lzo.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qkl.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blw.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aob.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eez.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ujo.andypj.xyz

Go:   // 手写循环累加
来源：http://mco.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://daa.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://mst.fehbvm.com

[D17] 最大值与最小值
来源：http://dhi.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://ttj.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://vsu.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vtv.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://veo.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://dwn.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bms.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://sru.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://ndr.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://qpp.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pyi.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://dpp.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qlu.guowangkeji.top

TS:   nested.flat();
来源：http://sju.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kki.daria6918.cn

Go:   // 手写双层循环
来源：http://bzb.aibaodan.cn

Ruby: nested.flatten
来源：http://tom.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ssg.xuanzx.com

[D19] 按字段分组
来源：http://ewv.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tnm.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wcz.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fbd.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mkx.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://emz.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://wrw.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qze.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://atj.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://kqq.fzhhl.top

Py:   Counter(arr)
来源：http://lgg.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://qrc.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avo.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lec.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ysl.cheryme.top

Go:   // 手写 map[T]int
来源：http://wng.yanxiufei.cn

Ruby: arr.tally
来源：http://dwd.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iue.ivvv.top

[D21] 判断是否包含某元素
来源：http://xlq.zhiwuduotai.top

Py:   x in arr
来源：http://xzg.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://sip.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://vsw.yongpay.top

TS:   arr.includes(x)
来源：http://jzt.hammf.cn

Java: list.contains(x)
来源：http://zfg.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ejf.ydzc1.top

Ruby: arr.include?(x)
来源：http://hgp.fktsv.cn

C#:   list.Contains(x)
来源：http://ucj.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://khb.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yxg.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eav.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sxe.gaohongyu789.top

TS:   [...arr];
来源：http://ssx.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://kfv.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xnb.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://otl.svipenyu.cn

C#:   new List<int>(list);
来源：http://ubm.tarul.cn

[D23] reduce 累积计算
来源：http://sjv.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yve.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tcd.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqe.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zah.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cwr.redwolf501.top

Go:   // 手写循环
来源：http://szp.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pog.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ofp.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://ggz.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://psd.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pvq.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mbf.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xak.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xmo.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jmb.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lvq.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sry.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://txo.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kvc.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rox.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ton.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uwp.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pxw.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zgb.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kdc.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ado.kuanghao11.cn

[D26] 数组转字符串
来源：http://kcn.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://zae.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://dxb.jinqigfzy.top

JS:   arr.join(", ")
来源：http://jyk.aibaodan.cn

TS:   arr.join(", ")
来源：http://wcp.aibaodan.cn

Java: String.join(", ", list)
来源：http://vtm.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://ohp.zhengqikj.top

Ruby: arr.join(", ")
来源：http://edz.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://gjw.hfpthk.cn

================================================================================
来源：http://egh.shanyushiyangtech.top

E. 字符串处理
来源：http://vle.daria6918.cn

================================================================================
来源：http://xsx.jlsjyb.cn

[E01] 拼接字符串
来源：http://uay.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tot.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://emd.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktg.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gzq.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uzi.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cnj.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rwy.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ljj.tian-w.cn

[E02] 重复字符串
来源：http://zeb.xziqi.cn

Py:   "ab" * 3
来源：http://ink.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://zez.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://czo.birdmap.top

TS:   "ab".repeat(3)
来源：http://vpn.0kj1m.cn

Java: "ab".repeat(3)
来源：http://gpq.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://tbn.dashuyun.cn

Ruby: "ab" * 3
来源：http://wit.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dvx.birdmap.top

[E03] 截取子串
来源：http://mbi.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wxg.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nmd.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zdu.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://mvw.316326.xyz

Java: s.substring(1, 4)
来源：http://fpm.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uzf.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://lxr.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://hbl.nanxuanxn.top

[E04] 查找子串位置
来源：http://ihc.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://enk.xuanzx.com

PHP:  strpos($s, "x");
来源：http://wcg.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xzi.pycfn.com

TS:   s.indexOf("x")
来源：http://xks.kuanghao11.cn

Java: s.indexOf("x")
来源：http://faf.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://mev.ydjk.org.cn

Ruby: s.index("x")
来源：http://nre.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://eoo.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://baa.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gng.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mle.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ubk.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nzo.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqg.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qtv.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lfx.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zvk.yj202588.top

[E06] 替换子串
来源：http://bjf.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://irz.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ufz.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://krn.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://wds.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqp.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jdy.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://crq.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://unq.jianghu66.top

[E07] 按分隔符拆分
来源：http://nzx.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sny.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://igw.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pqq.hysaishi.cn

TS:   s.split(",")
来源：http://ewa.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://itw.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wzk.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://gfu.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gkd.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://myv.pengpengdd.cyou

Py:   ",".join(items)
来源：http://ixj.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://rrg.nanxinkj.top

JS:   items.join(",")
来源：http://orv.pengpengdd.cyou

TS:   items.join(",")
来源：http://ezt.pycfn.com

Java: String.join(",", items)
来源：http://qof.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://eme.daria6918.cn

Ruby: items.join(",")
来源：http://kcu.52xcode.cn

C#:   string.Join(",", items)
来源：http://umn.iojbl.cn

[E09] 去除所有空白字符
来源：http://tga.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tty.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bbk.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://sjt.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://zhi.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://ymi.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://awe.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://mjy.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://szo.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://xqf.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://exk.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gkz.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://fql.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://fsn.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://rxr.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zfl.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qnd.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qsa.316326.xyz

[E11] 反转字符串
来源：http://tkv.mhx1999.top

Py:   s[::-1]
来源：http://khx.jinqigufen.top

PHP:  strrev($s);
来源：http://pkr.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://knp.tarul.cn

TS:   [...s].reverse().join("")
来源：http://ldv.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://yto.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tnr.tanke756.top

Ruby: s.reverse
来源：http://ffq.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pwm.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://wve.ehwqpu.com

Py:   s.count("a")
来源：http://tvv.316326.xyz

PHP:  substr_count($s, "a");
来源：http://wpo.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://eee.daria6918.cn

TS:   s.split("a").length - 1
来源：http://wdn.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jrg.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://gnd.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://pzw.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://igp.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://szr.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://dlc.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hxx.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://alq.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://eys.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgz.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://utz.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qrx.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pka.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://thh.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fuc.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ilm.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ybv.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gmv.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aqv.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uqr.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qhm.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqt.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://tyo.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hzp.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vbv.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wfg.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nzf.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qkg.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hnd.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbw.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qix.uphjek.com

[E16] 数字千分位
来源：http://rhp.fzhhl.top

Py:   f"{1234567:,}"
来源：http://gcp.hnqzz.top

PHP:  number_format(1234567);
来源：http://xmz.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hmz.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lnn.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lpg.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lgc.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wpf.yongpay.top

C#:   1234567.ToString("N0")
来源：http://qzy.andypj.xyz

[E17] 首字母大写
来源：http://xmb.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xwl.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dix.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cbn.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fgz.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://otg.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rws.bbcook.cn

Ruby: s.capitalize
来源：http://qkh.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dag.nanxuanxn.top

[E18] 模板占位符替换
来源：http://csn.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kyu.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yqz.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eru.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kdv.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fhu.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bmt.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mig.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ocg.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://bwl.fktsv.cn

Py:   s.splitlines()
来源：http://uea.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kmz.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://rld.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://hdi.xziqi.cn

Java: s.lines().toList()
来源：http://ifm.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://anq.xinyue.icu

Ruby: s.lines
来源：http://bip.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://jib.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://xte.daxiang520.top

Py:   if not s:
来源：http://plp.yfazqb.com


<!-- 参考信息 -->