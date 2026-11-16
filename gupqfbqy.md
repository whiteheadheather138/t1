代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wwr.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://iqp.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://kqr.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://akd.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tfj.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://zzl.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://emy.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://qot.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zng.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pxz.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://aaw.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://iyj.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ujl.mhx1999.top

Go:   // 手写循环
来源：http://mfh.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://dtz.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zkf.jianghu66.top

[D15] 去重
来源：http://rsy.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ews.chenlongwang.top

PHP:  array_unique($arr);
来源：http://dts.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://dzi.316326.xyz

TS:   [...new Set(arr)]
来源：http://fcf.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zgh.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://boe.fktsv.cn

Ruby: arr.uniq
来源：http://tgz.uphjek.com

C#:   list.Distinct().ToList()
来源：http://yfz.guannengcc.top

[D16] 求和与平均值
来源：http://rnb.quarkkingdee.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eui.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tjd.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuu.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://feq.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kun.daxiang520.top

Go:   // 手写循环累加
来源：http://wwn.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sht.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://bwe.wangdashe.top

[D17] 最大值与最小值
来源：http://kci.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://zjq.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://kba.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ntd.jinqigufen.top

TS:   Math.max(...arr);
来源：http://nkb.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eky.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ayj.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://fuq.tanke756.top

C#:   list.Max();  list.Min()
来源：http://nkq.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://olk.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mvt.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://bph.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dfo.shuidangran.top

TS:   nested.flat();
来源：http://xjq.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qgo.fengsongda.top

Go:   // 手写双层循环
来源：http://dzy.vqdsnc.cn

Ruby: nested.flatten
来源：http://gez.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dts.aizwys.cn

[D19] 按字段分组
来源：http://ztw.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jsc.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bjy.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eha.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vei.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rcj.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://djp.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zbp.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jyh.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://zwe.sufxvd.cn

Py:   Counter(arr)
来源：http://ycp.yj202588.top

PHP:  array_count_values($arr);
来源：http://kqn.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkv.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhe.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://odl.yueranfly.top

Go:   // 手写 map[T]int
来源：http://xeg.52xcode.cn

Ruby: arr.tally
来源：http://niu.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xem.bjfxy.top

[D21] 判断是否包含某元素
来源：http://vjh.hnxiangtu.top

Py:   x in arr
来源：http://qyi.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://zba.fzhhl.top

JS:   arr.includes(x)
来源：http://pxz.jyoumei.cn

TS:   arr.includes(x)
来源：http://fty.feifeiyinyue.top

Java: list.contains(x)
来源：http://nrk.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://cuf.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://evd.svipenyu.cn

C#:   list.Contains(x)
来源：http://tuu.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://xmb.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bnt.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nrv.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tgc.fanxiaobao.xyz

TS:   [...arr];
来源：http://wzt.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://xph.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://tsc.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://byf.fengsongda.top

C#:   new List<int>(list);
来源：http://qof.guowangkeji.top

[D23] reduce 累积计算
来源：http://kub.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hlj.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qkd.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hmt.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iws.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nac.guowangkeji.top

Go:   // 手写循环
来源：http://ham.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://var.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uih.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://vft.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jdo.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yke.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mur.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yjv.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tqx.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oxk.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tyh.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jpc.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://wbl.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ywn.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zkr.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://arc.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://poa.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kfu.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://elt.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwc.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cdu.sjlbkw.cn

[D26] 数组转字符串
来源：http://efo.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://jqk.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://wbg.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://xmo.jqgufenzy.top

TS:   arr.join(", ")
来源：http://xyl.bjfxy.top

Java: String.join(", ", list)
来源：http://abe.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://bpy.9152youxi.cn

Ruby: arr.join(", ")
来源：http://sig.fehbvm.com

C#:   string.Join(", ", list)
来源：http://yap.ywan-chungtsiang.top

================================================================================
来源：http://rgb.shangyingyoupin.top

E. 字符串处理
来源：http://ime.9152youxi.cn

================================================================================
来源：http://fzl.gogol.net.cn

[E01] 拼接字符串
来源：http://mzb.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wfl.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbm.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vei.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rhf.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vlm.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ybe.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kva.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xqa.snrcjt.cn

[E02] 重复字符串
来源：http://qje.yj20258888.top

Py:   "ab" * 3
来源：http://kkd.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://itq.birdmap.top

JS:   "ab".repeat(3)
来源：http://arq.sysykeji.top

TS:   "ab".repeat(3)
来源：http://vpa.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://knr.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://gag.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://cnl.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zfu.0kj1m.cn

[E03] 截取子串
来源：http://dip.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ojz.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://msu.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lep.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://kqs.sweek.top

Java: s.substring(1, 4)
来源：http://gum.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fkb.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dsm.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://akp.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://hpt.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://xbc.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://jyn.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hbi.redwolf501.top

TS:   s.indexOf("x")
来源：http://jys.meibo888.top

Java: s.indexOf("x")
来源：http://tia.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://wsd.iojbl.cn

Ruby: s.index("x")
来源：http://ckk.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://ggf.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opv.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eip.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rws.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vdp.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jae.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnj.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qke.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pwu.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vvo.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://zvv.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cfa.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://yyn.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://stj.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://pau.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wza.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cxj.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qig.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://mtw.nanxinkj.top

[E07] 按分隔符拆分
来源：http://wds.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mxh.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://otf.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cyn.meibo888.top

TS:   s.split(",")
来源：http://sig.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jcr.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://agy.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://qcr.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cxu.xziqi.cn

[E08] 数组按分隔符合并
来源：http://spr.wangdashe.top

Py:   ",".join(items)
来源：http://pav.havefunace.top

PHP:  implode(",", $items);
来源：http://cok.vehdjk.com

JS:   items.join(",")
来源：http://zsq.cqqwz.cn

TS:   items.join(",")
来源：http://sfx.zhijiandao.cn

Java: String.join(",", items)
来源：http://rql.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://dnq.zhongyouzk.top

Ruby: items.join(",")
来源：http://qxj.sweek.top

C#:   string.Join(",", items)
来源：http://gda.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://nkq.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bla.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wmp.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://lza.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://dul.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xig.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://anp.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ylm.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cfa.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://tbx.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vud.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jzo.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://cox.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://hbb.yj20258888.top

Java: String.format("%03d", 7)
来源：http://asq.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmw.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fon.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nea.wangshuangyany.cn

[E11] 反转字符串
来源：http://jfd.svipenyu.cn

Py:   s[::-1]
来源：http://qev.jqgufenzy.top

PHP:  strrev($s);
来源：http://ovl.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://vog.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://xvy.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://fkq.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hbd.nanxuanxn.top

Ruby: s.reverse
来源：http://mrv.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wnv.0kj1m.cn

[E12] 统计某字符出现次数
来源：http://iqb.wangshuangyany.cn

Py:   s.count("a")
来源：http://blm.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://hyp.cashguo.top

JS:   s.split("a").length - 1
来源：http://xko.pycfn.com

TS:   s.split("a").length - 1
来源：http://qco.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iuh.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://ehm.fktsv.cn

Ruby: s.count("a")
来源：http://hal.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://ihz.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://qlb.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://bfd.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zwr.shzxlz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gts.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mbq.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xyu.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dpu.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aar.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gte.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://cdq.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ecw.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rbg.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ssi.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wyt.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edp.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://egy.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yra.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://efg.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://nsg.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://giy.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqn.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbt.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pld.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://akr.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zaf.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pkn.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zms.ppjwa.cn

[E16] 数字千分位
来源：http://kfj.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://xva.ydzc1.top

PHP:  number_format(1234567);
来源：http://eqo.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mit.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ehj.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://veg.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zbz.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vny.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://ttf.hammf.cn

[E17] 首字母大写
来源：http://ffd.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vqn.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://osb.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnh.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvm.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hdf.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://svn.daxiang520.top

Ruby: s.capitalize
来源：http://ctw.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvb.yuxming.cn

[E18] 模板占位符替换
来源：http://isb.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dem.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zyu.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://ixg.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qcj.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ufs.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xit.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://whr.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cyq.mhx1999.top

[E19] 多行文本按行拆分
来源：http://wsg.tarul.cn

Py:   s.splitlines()
来源：http://czk.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ltw.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://knw.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://pbz.andypj.xyz

Java: s.lines().toList()
来源：http://zpa.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://fay.snrcjt.cn

Ruby: s.lines
来源：http://ozk.sysykeji.top

C#:   s.Split('\n')
来源：http://qym.yvedp.cn

[E20] 判断字符串是否为空
来源：http://rko.iojbl.cn

Py:   if not s:
来源：http://uih.hongshengwenyu.top


<!-- 参考信息 -->