代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xzq.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://rmr.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://wou.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://huc.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yta.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ksi.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wfo.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://orf.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fhz.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jzn.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://zda.hnxiangtu.top

TS:   arr.map(x => x * 2)
来源：http://ixt.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rdp.shanyushiyangtech.top

Go:   // 手写循环
来源：http://woo.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nzp.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wrg.hywenlv.cn

[D15] 去重
来源：http://itn.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://riv.cucudq.cn

PHP:  array_unique($arr);
来源：http://wde.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://ckw.bjfxy.top

TS:   [...new Set(arr)]
来源：http://ywz.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sea.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://whq.hywenlv.cn

Ruby: arr.uniq
来源：http://cvj.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://djd.dashuyun.cn

[D16] 求和与平均值
来源：http://kkx.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xol.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vom.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://asa.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqe.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ojl.dianchejie.cn

Go:   // 手写循环累加
来源：http://bae.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ikb.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://cpt.chenlongwang.top

[D17] 最大值与最小值
来源：http://tlr.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://kbz.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://vpx.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yuk.shuidangran.top

TS:   Math.max(...arr);
来源：http://gqh.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xko.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zax.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://klc.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://qhx.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://zjj.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://otg.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://iqk.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tzd.haohaochexian.top

TS:   nested.flat();
来源：http://zem.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fms.wangdashe.top

Go:   // 手写双层循环
来源：http://moo.bbcook.cn

Ruby: nested.flatten
来源：http://ohd.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsa.vehdjk.com

[D19] 按字段分组
来源：http://rca.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxc.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yfi.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dcq.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ltr.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dhc.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://lqh.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fft.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fqk.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://hmr.chenlongwang.top

Py:   Counter(arr)
来源：http://nyw.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://ppb.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://waq.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jts.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bfn.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://hjy.9152youxi.cn

Ruby: arr.tally
来源：http://emb.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uko.smart0.xyz

[D21] 判断是否包含某元素
来源：http://iag.wangshuangyany.cn

Py:   x in arr
来源：http://wqg.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://ffn.ehwqpu.com

JS:   arr.includes(x)
来源：http://bbm.cheryme.top

TS:   arr.includes(x)
来源：http://ezm.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://cdc.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://hkz.52xcode.cn

Ruby: arr.include?(x)
来源：http://dsl.yangfankeji.com

C#:   list.Contains(x)
来源：http://tro.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://yae.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://orr.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gxa.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ott.yonumen.top

TS:   [...arr];
来源：http://pxr.yfazqb.com

Java: new ArrayList<>(list);
来源：http://ydl.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://ero.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://tok.316326.xyz

C#:   new List<int>(list);
来源：http://ylu.jyoumei.cn

[D23] reduce 累积计算
来源：http://jwm.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://znw.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yhe.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qli.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxv.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://srm.uphjek.com

Go:   // 手写循环
来源：http://swo.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qbp.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://faa.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://asr.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mgg.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kqv.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xba.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qoq.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://csu.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uuz.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbs.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lbu.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://zgg.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bht.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kkk.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mqx.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ehg.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mww.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qau.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mqx.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqp.shuidangran.top

[D26] 数组转字符串
来源：http://aax.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://int.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://thm.zhoulong.xyz

JS:   arr.join(", ")
来源：http://bih.gotoacloud.top

TS:   arr.join(", ")
来源：http://erb.fengsongda.top

Java: String.join(", ", list)
来源：http://fgi.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://xhs.dashuyun.cn

Ruby: arr.join(", ")
来源：http://mwz.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://jcu.bbcook.cn

================================================================================
来源：http://rij.xuanzx.com

E. 字符串处理
来源：http://dqa.shuidangran.top

================================================================================
来源：http://txt.dashuyun.cn

[E01] 拼接字符串
来源：http://xsa.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xxf.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mcb.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://owo.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rvs.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bvu.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zuy.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xbp.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mux.cucudq.cn

[E02] 重复字符串
来源：http://bcp.zhongyouzk.top

Py:   "ab" * 3
来源：http://gbl.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://oxc.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://jlo.ybcxt.top

TS:   "ab".repeat(3)
来源：http://mna.redwolf501.top

Java: "ab".repeat(3)
来源：http://cpq.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://afp.hnqzz.top

Ruby: "ab" * 3
来源：http://xip.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mwf.jqgufenzy.top

[E03] 截取子串
来源：http://iep.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rhv.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uvi.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qgr.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://imy.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://phs.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ryp.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://chg.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://pye.zycfv.cn

[E04] 查找子串位置
来源：http://vcn.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://rpp.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://luj.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://puw.cheryme.top

TS:   s.indexOf("x")
来源：http://mtw.316326.xyz

Java: s.indexOf("x")
来源：http://ezr.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://ctx.chenzaomai.com

Ruby: s.index("x")
来源：http://dnn.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://ceh.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bpo.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yzh.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ast.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgn.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://wvk.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oyr.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tiy.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://miz.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vaq.sxryk.cn

[E06] 替换子串
来源：http://nof.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://udp.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://fca.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rxa.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://tdf.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngk.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://smj.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmi.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://jxl.guowangkeji.top

[E07] 按分隔符拆分
来源：http://raa.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kdx.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vnw.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qob.redwolf501.top

TS:   s.split(",")
来源：http://vgn.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://reb.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://egi.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://vsz.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://spr.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://cfm.hfpthk.cn

Py:   ",".join(items)
来源：http://yxl.andypj.xyz

PHP:  implode(",", $items);
来源：http://ukv.cheryme.top

JS:   items.join(",")
来源：http://swi.ybcxt.top

TS:   items.join(",")
来源：http://ioy.jqgufenzy.top

Java: String.join(",", items)
来源：http://boc.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://iun.tian-w.cn

Ruby: items.join(",")
来源：http://fxf.zdqjudy.top

C#:   string.Join(",", items)
来源：http://yai.iojbl.cn

[E09] 去除所有空白字符
来源：http://qrf.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rpv.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://miw.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://jas.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://ami.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rdk.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://edi.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://liu.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ykz.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://rio.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rsg.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zyi.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://pwx.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://pyb.yuxming.cn

Java: String.format("%03d", 7)
来源：http://hbt.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wbi.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pit.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dis.zhijiandao.cn

[E11] 反转字符串
来源：http://vtv.wangshuangyany.cn

Py:   s[::-1]
来源：http://xxq.xuetiantiany.cn

PHP:  strrev($s);
来源：http://uht.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://ime.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://lsf.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xsm.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://udc.feifeiyinyue.top

Ruby: s.reverse
来源：http://iek.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dkb.fktsv.cn

[E12] 统计某字符出现次数
来源：http://dfr.hammf.cn

Py:   s.count("a")
来源：http://zpy.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://lzr.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://qdn.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://sua.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qcu.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://gkp.xuetiantiany.cn

Ruby: s.count("a")
来源：http://gxg.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://gmc.shzxlz.cn

[E13] 逐字符遍历
来源：http://jta.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://dka.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pad.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://itk.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lda.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aar.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vkl.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mup.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hgi.wangdashe.top

[E14] URL 编码与 Base64
来源：http://fph.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tov.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://oqt.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ndj.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xdb.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bnk.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://srb.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ocj.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpp.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://bqc.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://lpz.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://udi.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rqr.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zxg.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jxk.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbr.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ref.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bsl.xuetiantiany.cn

[E16] 数字千分位
来源：http://xjt.pycfn.com

Py:   f"{1234567:,}"
来源：http://lrw.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://iye.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gus.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ctm.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mzs.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ihr.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jrl.tarul.cn

C#:   1234567.ToString("N0")
来源：http://rua.bjfxy.top

[E17] 首字母大写
来源：http://uvh.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dji.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ein.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rwe.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzx.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ubt.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zzk.daria6918.cn

Ruby: s.capitalize
来源：http://qrd.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ndy.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://gcm.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mlz.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rbq.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bin.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://don.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ivb.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hvl.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://msj.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vpo.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://zat.zhiwuduotai.top

Py:   s.splitlines()
来源：http://fph.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bcn.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://tsn.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://qgq.guowangkeji.top

Java: s.lines().toList()
来源：http://xpr.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://iat.shanyushiyangtech.top

Ruby: s.lines
来源：http://yrc.ehwqpu.com

C#:   s.Split('\n')
来源：http://uxm.yj202588.top

[E20] 判断字符串是否为空
来源：http://ofa.316326.xyz

Py:   if not s:
来源：http://mzz.hongshengwenyu.top


<!-- 参考信息 -->