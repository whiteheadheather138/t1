代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyt.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tmu.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vig.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://eyy.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tet.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ysm.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://cmq.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://buj.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ybg.sufxvd.cn

Go:   // 手写循环
来源：http://pjm.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dlx.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fcb.sysykeji.top

[D15] 去重
来源：http://htu.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ovf.sxryk.cn

PHP:  array_unique($arr);
来源：http://sjc.shuidangran.top

JS:   [...new Set(arr)]
来源：http://aqo.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://mik.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://epv.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kxy.zdbjq.cn

Ruby: arr.uniq
来源：http://knk.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://bcc.nanxuanxn.top

[D16] 求和与平均值
来源：http://gzj.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mwv.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jvu.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wox.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afu.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fit.gzhubu.top

Go:   // 手写循环累加
来源：http://pvw.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://khl.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://pqf.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://pov.cashguo.top

Py:   max(arr);  min(arr)
来源：http://xam.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://zfn.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ndz.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://hyv.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fup.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vdd.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://dzv.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://rcc.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://lki.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zuu.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://xjp.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mhi.yueranfly.top

TS:   nested.flat();
来源：http://xqf.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://anw.fzhhl.top

Go:   // 手写双层循环
来源：http://utv.xziqi.cn

Ruby: nested.flatten
来源：http://cqw.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://snp.yangfankeji.com

[D19] 按字段分组
来源：http://dlg.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://isp.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gcj.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gly.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tqo.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tet.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://vcx.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vop.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vnk.yongpay.top

[D20] 统计每个元素出现次数
来源：http://iqi.zhoulong.xyz

Py:   Counter(arr)
来源：http://azq.yongpay.top

PHP:  array_count_values($arr);
来源：http://zti.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjo.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://icg.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pjc.cheryme.top

Go:   // 手写 map[T]int
来源：http://ked.zhixingplan.top

Ruby: arr.tally
来源：http://zkv.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ape.uphjek.com

[D21] 判断是否包含某元素
来源：http://tkj.fanxiaobao.xyz

Py:   x in arr
来源：http://pfb.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://umq.tanke756.top

JS:   arr.includes(x)
来源：http://udp.ybcxt.top

TS:   arr.includes(x)
来源：http://ogy.vqdsnc.cn

Java: list.contains(x)
来源：http://ttx.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://xjc.shuidangran.top

Ruby: arr.include?(x)
来源：http://qul.zycfv.cn

C#:   list.Contains(x)
来源：http://jgb.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://utx.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://isw.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jvy.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kcv.ydjk.org.cn

TS:   [...arr];
来源：http://qmb.tanke756.top

Java: new ArrayList<>(list);
来源：http://twi.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cig.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://jss.jinqigufen.top

C#:   new List<int>(list);
来源：http://prb.nanxinkj.top

[D23] reduce 累积计算
来源：http://efq.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://prf.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tjf.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ree.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lqh.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qmt.hongshengwenyu.top

Go:   // 手写循环
来源：http://msy.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qew.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ngm.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://ayf.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://umr.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blm.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svm.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cno.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qtf.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lzr.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbz.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sba.cashguo.top

[D25] Set 集合去重与交并差
来源：http://see.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fao.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cad.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eet.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gsc.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bqm.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ldo.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aec.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kdu.9152youxi.cn

[D26] 数组转字符串
来源：http://mgq.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://hef.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://oqy.xinyue.icu

JS:   arr.join(", ")
来源：http://fme.sufxvd.cn

TS:   arr.join(", ")
来源：http://kbp.zhijiandao.cn

Java: String.join(", ", list)
来源：http://nzl.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://edk.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://qem.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://gnc.jinqigfzy.top

================================================================================
来源：http://yhb.ivvv.top

E. 字符串处理
来源：http://ycp.jqgfzy.top

================================================================================
来源：http://rcy.epnwcf.com

[E01] 拼接字符串
来源：http://vcd.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hkw.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zou.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kqn.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlp.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://arh.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ilb.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wjw.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uyf.ivvv.top

[E02] 重复字符串
来源：http://ket.feifeiyinyue.top

Py:   "ab" * 3
来源：http://nqv.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://bty.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://xry.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://ccd.chenzaomai.com

Java: "ab".repeat(3)
来源：http://fkp.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://ewn.hesvh.cn

Ruby: "ab" * 3
来源：http://xft.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dej.quarkkingdee.top

[E03] 截取子串
来源：http://efl.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sbp.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gam.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqt.daxiang520.top

TS:   s.slice(1, 4)
来源：http://lhg.52xcode.cn

Java: s.substring(1, 4)
来源：http://qrc.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://thv.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://prf.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://qka.sjlbkw.cn

[E04] 查找子串位置
来源：http://fpa.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://dun.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://iyg.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vys.hywenlv.cn

TS:   s.indexOf("x")
来源：http://loa.zhongyouzk.top

Java: s.indexOf("x")
来源：http://lgh.ivvv.top

Go:   strings.Index(s, "x")
来源：http://bpr.pycfn.com

Ruby: s.index("x")
来源：http://lph.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://tmz.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bes.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lyn.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yal.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jnb.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hdf.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjt.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vxq.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vra.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nif.chenjidiqi.icu

[E06] 替换子串
来源：http://kvy.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://upi.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://rrd.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idt.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://fvt.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcn.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eyl.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ldw.cheryme.top

C#:   s.Replace("a", "b")
来源：http://qjk.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://axz.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yqt.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bqp.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://him.hnxiangtu.top

TS:   s.split(",")
来源：http://hur.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://bdm.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wol.tanke756.top

Ruby: s.split(",");  s.split
来源：http://gxh.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vub.fzhhl.top

[E08] 数组按分隔符合并
来源：http://ynf.xylfe.cn

Py:   ",".join(items)
来源：http://tmh.hfpthk.cn

PHP:  implode(",", $items);
来源：http://smt.bbcook.cn

JS:   items.join(",")
来源：http://fjg.andypj.xyz

TS:   items.join(",")
来源：http://hjn.tanke756.top

Java: String.join(",", items)
来源：http://wcb.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://wow.snrcjt.cn

Ruby: items.join(",")
来源：http://gdx.yuanzhike.top

C#:   string.Join(",", items)
来源：http://qka.mhx1999.top

[E09] 去除所有空白字符
来源：http://vhf.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tao.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pon.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://tpb.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://fvx.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://djp.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zfq.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://ppb.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ctp.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://nxw.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rxq.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ulw.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://qgi.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://qmf.fktsv.cn

Java: String.format("%03d", 7)
来源：http://lap.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftj.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tlu.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxt.shanyushiyangtech.top

[E11] 反转字符串
来源：http://uhx.smart0.xyz

Py:   s[::-1]
来源：http://bls.c1oappe.top

PHP:  strrev($s);
来源：http://yza.cheryme.top

JS:   [...s].reverse().join("")
来源：http://isl.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://lcf.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eun.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://voy.shuidangran.top

Ruby: s.reverse
来源：http://zts.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://zcb.hammf.cn

[E12] 统计某字符出现次数
来源：http://vfo.vqdsnc.cn

Py:   s.count("a")
来源：http://hyl.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://mpv.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://qvb.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://het.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bij.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://aed.bbcook.cn

Ruby: s.count("a")
来源：http://rif.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://zdp.hesvh.cn

[E13] 逐字符遍历
来源：http://ycr.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://ril.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fkf.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oyq.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ida.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mcs.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ifd.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zvi.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lct.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://wfb.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hmb.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cjb.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://moz.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mwa.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fux.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zmx.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qem.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kbj.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://abc.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vjw.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mct.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://etu.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://msc.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://llk.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ddq.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vyt.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fkr.andypj.xyz

[E16] 数字千分位
来源：http://hlx.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://nhj.hysaishi.cn

PHP:  number_format(1234567);
来源：http://mxt.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gvk.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wdh.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mxh.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://npe.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ven.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://gho.dashuyun.cn

[E17] 首字母大写
来源：http://svr.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rqw.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wvy.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fsq.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eui.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ylr.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jfs.zycfv.cn

Ruby: s.capitalize
来源：http://hal.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fsn.birdmap.top

[E18] 模板占位符替换
来源：http://opo.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://phb.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://auw.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lln.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://phi.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eaj.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vba.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ieh.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mvu.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://yhg.tanke756.top

Py:   s.splitlines()
来源：http://dte.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sjo.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://omh.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://ryy.pengpengdd.cyou

Java: s.lines().toList()
来源：http://wtj.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://hno.tarul.cn

Ruby: s.lines
来源：http://qnz.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://jzn.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://rzb.vqdsnc.cn

Py:   if not s:
来源：http://ggs.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mbw.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jsf.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://hxa.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://hhi.feifeiyinyue.top


<!-- 参考信息 -->