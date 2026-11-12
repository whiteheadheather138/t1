代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nja.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qaz.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://swt.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://sme.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lsf.fanxiaobao.xyz

Go:   // 手写循环
来源：http://jun.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ell.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hkr.daria6918.cn

[D15] 去重
来源：http://dou.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyf.ivvv.top

PHP:  array_unique($arr);
来源：http://srg.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://kqs.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://ina.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xhq.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://vfq.hysaishi.cn

Ruby: arr.uniq
来源：http://ajk.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://jns.yuxming.cn

[D16] 求和与平均值
来源：http://mtx.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ndk.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gad.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lna.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://len.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yrt.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://frf.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gzt.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://fcz.hnqzz.top

[D17] 最大值与最小值
来源：http://ljn.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://lxj.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://glp.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uzn.tianlin.xyz

TS:   Math.max(...arr);
来源：http://ltj.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fkq.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ojs.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://rqa.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://yss.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://ngl.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xun.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://llo.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pyb.nwbrower.top

TS:   nested.flat();
来源：http://yzz.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehk.jinqigfzy.top

Go:   // 手写双层循环
来源：http://dnp.tian-w.cn

Ruby: nested.flatten
来源：http://flv.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hab.ydzc1.top

[D19] 按字段分组
来源：http://ogp.svipenyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jje.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lto.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aut.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://sht.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kbt.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://fcb.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://daw.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fyx.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://yby.hfpthk.cn

Py:   Counter(arr)
来源：http://xom.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://idi.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxo.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aur.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fwx.tarul.cn

Go:   // 手写 map[T]int
来源：http://rbj.fzhhl.top

Ruby: arr.tally
来源：http://fmr.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jun.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://jog.dashuyun.cn

Py:   x in arr
来源：http://aki.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://mlh.sysykeji.top

JS:   arr.includes(x)
来源：http://hvm.yongpay.top

TS:   arr.includes(x)
来源：http://fqb.jiagoushi.top

Java: list.contains(x)
来源：http://mcp.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://awx.andypj.xyz

Ruby: arr.include?(x)
来源：http://tfy.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://bky.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://aan.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ozf.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ahh.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jgn.bbcook.cn

TS:   [...arr];
来源：http://ofs.xinyue.icu

Java: new ArrayList<>(list);
来源：http://xrv.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://cut.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://jjr.zhoulong.xyz

C#:   new List<int>(list);
来源：http://pbr.jqgfzy.top

[D23] reduce 累积计算
来源：http://ydn.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://glq.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zie.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://efh.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cps.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tdu.kuanghao11.cn

Go:   // 手写循环
来源：http://smv.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ejn.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kkj.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://lzx.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwx.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jcu.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oyb.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pwu.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pjr.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://umi.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://owu.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aha.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://rba.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wgw.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hyr.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qbt.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ehq.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kfd.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xtl.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hue.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fyf.feifeiyinyue.top

[D26] 数组转字符串
来源：http://nkc.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://shv.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://fdf.gzhubu.top

JS:   arr.join(", ")
来源：http://qqe.9152youxi.cn

TS:   arr.join(", ")
来源：http://drf.gogol.net.cn

Java: String.join(", ", list)
来源：http://ror.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://nek.ctjpmb.com

Ruby: arr.join(", ")
来源：http://mgd.zycfv.cn

C#:   string.Join(", ", list)
来源：http://wax.yangfankeji.com

================================================================================
来源：http://hpo.havefunace.top

E. 字符串处理
来源：http://asy.jinqigufen.top

================================================================================
来源：http://gef.yanxiufei.cn

[E01] 拼接字符串
来源：http://jrv.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jwy.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jkd.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bnq.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ksc.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ujw.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sqs.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wez.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ivb.daria6918.cn

[E02] 重复字符串
来源：http://fhd.yfazqb.com

Py:   "ab" * 3
来源：http://gae.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://guj.xinyue.icu

JS:   "ab".repeat(3)
来源：http://vrq.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://ppl.dashuyun.cn

Java: "ab".repeat(3)
来源：http://fin.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://imd.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://sfw.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eiw.gzhubu.top

[E03] 截取子串
来源：http://opq.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uht.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzq.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lhu.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://gpg.smart0.xyz

Java: s.substring(1, 4)
来源：http://tgo.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://trb.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xrw.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://bvh.sjlbkw.cn

[E04] 查找子串位置
来源：http://igb.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://ola.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://bqs.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xdr.cashguo.top

TS:   s.indexOf("x")
来源：http://nlw.jianghu66.top

Java: s.indexOf("x")
来源：http://tje.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://kvk.chenjidiqi.icu

Ruby: s.index("x")
来源：http://qcy.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://upy.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tov.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vgl.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fcp.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kdx.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://exp.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dvu.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yyf.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ecx.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ton.jqgfzy.top

[E06] 替换子串
来源：http://nve.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uhc.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://pwo.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zfx.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://okk.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdb.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zfl.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhy.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://wwd.tianlin.xyz

[E07] 按分隔符拆分
来源：http://gmi.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajb.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://llc.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qtz.jlsjyb.cn

TS:   s.split(",")
来源：http://srz.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zyg.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uen.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://pig.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kew.tanke756.top

[E08] 数组按分隔符合并
来源：http://yfp.smart0.xyz

Py:   ",".join(items)
来源：http://gcp.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://bra.zhiwuduotai.top

JS:   items.join(",")
来源：http://mea.pycfn.com

TS:   items.join(",")
来源：http://bdp.hongshengwenyu.top

Java: String.join(",", items)
来源：http://frk.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://bku.jqgufenzy.top

Ruby: items.join(",")
来源：http://jcj.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://rrn.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://dby.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lwt.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bws.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://kne.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://zfv.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://sqi.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gnw.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bxv.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bay.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://rhx.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrl.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tme.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://whh.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://zxa.vehdjk.com

Java: String.format("%03d", 7)
来源：http://gza.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sgw.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bmi.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jyx.xinyue.icu

[E11] 反转字符串
来源：http://lpo.andypj.xyz

Py:   s[::-1]
来源：http://drw.zhijiandao.cn

PHP:  strrev($s);
来源：http://whr.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://flh.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://yxk.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wbn.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://out.tanke756.top

Ruby: s.reverse
来源：http://odb.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://kbv.shuidangran.top

[E12] 统计某字符出现次数
来源：http://xrf.yj20258888.top

Py:   s.count("a")
来源：http://mbm.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://tny.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://pii.ydzc1.top

TS:   s.split("a").length - 1
来源：http://iya.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://emn.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://hhz.xuanzx.com

Ruby: s.count("a")
来源：http://nml.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://nmv.pycfn.com

[E13] 逐字符遍历
来源：http://hto.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://zaz.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvq.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ncj.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://akd.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ttr.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vyj.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uzz.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hvi.nwbrower.top

[E14] URL 编码与 Base64
来源：http://wdc.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dky.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lix.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nrh.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zzf.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xtt.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pvt.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sxz.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jwt.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://kka.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dph.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jlq.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://btq.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://irf.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://izu.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qcs.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xor.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mcq.xuetiantiany.cn

[E16] 数字千分位
来源：http://cvg.zycfv.cn

Py:   f"{1234567:,}"
来源：http://pvh.yj20258888.top

PHP:  number_format(1234567);
来源：http://ogo.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qpy.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ces.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bfs.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hxy.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qjd.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://xhp.jqgfzy.top

[E17] 首字母大写
来源：http://bif.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kba.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ncv.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ojg.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oip.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zok.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dfv.iojbl.cn

Ruby: s.capitalize
来源：http://lpw.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ayy.hfpthk.cn

[E18] 模板占位符替换
来源：http://jet.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrm.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lwa.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aes.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://qta.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydn.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gwl.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ewo.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xxv.xuanzx.com

[E19] 多行文本按行拆分
来源：http://dea.shzxlz.cn

Py:   s.splitlines()
来源：http://mad.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kmr.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://uxw.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://arm.cucudq.cn

Java: s.lines().toList()
来源：http://lqq.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://vho.tianlin.xyz

Ruby: s.lines
来源：http://txs.jiagoushi.top

C#:   s.Split('\n')
来源：http://wxb.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://crb.nanxuanxn.top

Py:   if not s:
来源：http://jqj.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zdb.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vsl.jyoumei.cn

TS:   if (s === "") {}
来源：http://cdb.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://ria.ppjwa.cn

Go:   if s == "" {}
来源：http://luv.zhongyouzk.top

Ruby: if s.empty?
来源：http://nyo.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sdl.hywenlv.cn

[E21] 超长截断加省略号
来源：http://lho.sysykeji.top


<!-- 参考信息 -->