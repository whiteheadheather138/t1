代发 wailian999

[D15] 去重
来源：http://kmi.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qnl.wangdashe.top

PHP:  array_unique($arr);
来源：http://hyf.wangdashe.top

JS:   [...new Set(arr)]
来源：http://qbq.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://goh.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hmp.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://sbn.zdbjq.cn

Ruby: arr.uniq
来源：http://pva.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://sok.redwolf501.top

[D16] 求和与平均值
来源：http://moi.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oja.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sos.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uhq.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ksz.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://soz.yongpay.top

Go:   // 手写循环累加
来源：http://ezu.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vol.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://mss.fengsongda.top

[D17] 最大值与最小值
来源：http://fxg.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://mzz.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://zly.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rrg.0kj1m.cn

TS:   Math.max(...arr);
来源：http://vxy.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cii.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dob.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://pdx.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ctv.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://xwn.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://adc.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://kzg.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fve.redwolf501.top

TS:   nested.flat();
来源：http://vfa.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yil.ydzc1.top

Go:   // 手写双层循环
来源：http://vgk.zhoulong.xyz

Ruby: nested.flatten
来源：http://vns.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pzx.vqdsnc.cn

[D19] 按字段分组
来源：http://hwe.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gdr.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pff.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubz.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ost.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzk.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://lzg.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oou.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tgy.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://lgu.316326.xyz

Py:   Counter(arr)
来源：http://tbr.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://etb.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aez.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwb.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jfy.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://gbp.hnqzz.top

Ruby: arr.tally
来源：http://nvs.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dii.fzhhl.top

[D21] 判断是否包含某元素
来源：http://sqj.xinyue.icu

Py:   x in arr
来源：http://fbc.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://hio.quarkkingdee.top

JS:   arr.includes(x)
来源：http://fwj.sweek.top

TS:   arr.includes(x)
来源：http://whw.shuidangran.top

Java: list.contains(x)
来源：http://wtv.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://nam.havefunace.top

Ruby: arr.include?(x)
来源：http://zer.yfazqb.com

C#:   list.Contains(x)
来源：http://cbj.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://trf.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iay.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mxu.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xiw.xinyue.icu

TS:   [...arr];
来源：http://ccg.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://cpy.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://keq.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://cfu.fktsv.cn

C#:   new List<int>(list);
来源：http://fuc.jinqigufen.top

[D23] reduce 累积计算
来源：http://wgd.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fcs.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ija.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ggf.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sdw.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://swg.andypj.xyz

Go:   // 手写循环
来源：http://zpe.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pjb.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://brp.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://orm.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hac.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wqh.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wqb.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://azl.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://myd.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fto.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ufp.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ifu.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://ijm.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nqf.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dnf.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qtn.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nfa.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mrx.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mty.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyc.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yde.jinqigufen.top

[D26] 数组转字符串
来源：http://uih.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://lmq.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://fco.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://qok.cdnleiting.top

TS:   arr.join(", ")
来源：http://mwy.gogol.net.cn

Java: String.join(", ", list)
来源：http://fvr.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://lnu.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://ykk.meibo888.top

C#:   string.Join(", ", list)
来源：http://oog.yongpay.top

================================================================================
来源：http://ztp.sufxvd.cn

E. 字符串处理
来源：http://srd.daxiang520.top

================================================================================
来源：http://dpz.zhoulong.xyz

[E01] 拼接字符串
来源：http://rxi.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tgv.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://naz.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://puz.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nrn.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vrs.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tpe.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qht.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oct.jqgfzy.top

[E02] 重复字符串
来源：http://mnx.0kj1m.cn

Py:   "ab" * 3
来源：http://oxh.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://ocf.nwbrower.top

JS:   "ab".repeat(3)
来源：http://hwd.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://pzq.aibaodan.cn

Java: "ab".repeat(3)
来源：http://dcc.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://mdn.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://fra.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://smy.hfpthk.cn

[E03] 截取子串
来源：http://shx.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hgs.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fqt.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xyd.yj20258888.top

TS:   s.slice(1, 4)
来源：http://mgp.zdqjudy.top

Java: s.substring(1, 4)
来源：http://edk.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fjx.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://ikd.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://csx.gaohongyu789.top

[E04] 查找子串位置
来源：http://uxi.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://bbm.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://vef.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wsw.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://piz.ybcxt.top

Java: s.indexOf("x")
来源：http://awu.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://fqo.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://yrh.xinyue.icu

C#:   s.IndexOf("x")
来源：http://fbf.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xym.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvo.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gqq.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cfm.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffo.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oia.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://buw.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yuy.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lvs.ivvv.top

[E06] 替换子串
来源：http://coz.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://les.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://kqw.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hzc.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://hgq.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ezx.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lqc.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzp.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://ikd.xinyue.icu

[E07] 按分隔符拆分
来源：http://saw.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://udk.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wpi.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yfa.gzhubu.top

TS:   s.split(",")
来源：http://zia.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://bgh.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nty.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://dds.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qdr.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://jsm.yongpay.top

Py:   ",".join(items)
来源：http://krf.pycfn.com

PHP:  implode(",", $items);
来源：http://drx.yangfankeji.com

JS:   items.join(",")
来源：http://yms.birdmap.top

TS:   items.join(",")
来源：http://eng.yuxming.cn

Java: String.join(",", items)
来源：http://mxc.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://oae.tarul.cn

Ruby: items.join(",")
来源：http://pom.mhx1999.top

C#:   string.Join(",", items)
来源：http://kah.fzhhl.top

[E09] 去除所有空白字符
来源：http://vyq.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwk.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wsf.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://usy.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rzn.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://lws.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zep.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zys.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sav.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://cfd.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sus.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwt.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://vrc.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://mmz.guannengcc.top

Java: String.format("%03d", 7)
来源：http://ego.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zot.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgm.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lab.jqgufenzy.top

[E11] 反转字符串
来源：http://nel.nanxuanxn.top

Py:   s[::-1]
来源：http://pfu.fzhhl.top

PHP:  strrev($s);
来源：http://uup.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://ihi.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://ydp.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jme.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zck.vehdjk.com

Ruby: s.reverse
来源：http://dgg.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kgd.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://sqy.quarkkingdee.top

Py:   s.count("a")
来源：http://xte.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://nqa.316326.xyz

JS:   s.split("a").length - 1
来源：http://ckf.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://fyv.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ert.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://fzh.fehbvm.com

Ruby: s.count("a")
来源：http://yqi.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://sdy.xylfe.cn

[E13] 逐字符遍历
来源：http://wkm.uphjek.com

Py:   for ch in s: print(ch)
来源：http://bju.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://scg.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dts.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kpq.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ybc.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jse.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://baf.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vdt.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://hmb.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwk.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uir.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wyh.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iwk.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zor.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cuv.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://smc.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swf.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://kgv.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pur.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cio.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pva.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sig.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://abb.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xgi.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lrl.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://spd.9152youxi.cn

[E16] 数字千分位
来源：http://dlk.guannengcc.top

Py:   f"{1234567:,}"
来源：http://zpd.uphjek.com

PHP:  number_format(1234567);
来源：http://gjv.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ghi.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ikj.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rvd.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxi.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mso.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://tpp.daxiang520.top

[E17] 首字母大写
来源：http://ckx.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eiq.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://rpn.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://myn.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvv.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://erd.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aiz.fzhhl.top

Ruby: s.capitalize
来源：http://tmb.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cll.cheryme.top

[E18] 模板占位符替换
来源：http://myz.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pfh.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fmr.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://rky.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mfr.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://erf.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qat.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hgu.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pjn.jianghu66.top

[E19] 多行文本按行拆分
来源：http://pjj.iojbl.cn

Py:   s.splitlines()
来源：http://ukm.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jzr.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://pjj.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://gfh.zhijiandao.cn

Java: s.lines().toList()
来源：http://ugb.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://eag.zhixingplan.top

Ruby: s.lines
来源：http://uta.aibaodan.cn

C#:   s.Split('\n')
来源：http://xhl.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://rrl.jinqigfzy.top

Py:   if not s:
来源：http://rhx.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zdq.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blp.zhijiandao.cn

TS:   if (s === "") {}
来源：http://izb.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://alw.yj20258.top

Go:   if s == "" {}
来源：http://juo.daria6918.cn

Ruby: if s.empty?
来源：http://rxf.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vzv.ehwqpu.com

[E21] 超长截断加省略号
来源：http://lsa.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hok.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tlh.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://csh.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nib.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emk.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://rjb.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://awg.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hwo.yfazqb.com


<!-- 参考信息 -->