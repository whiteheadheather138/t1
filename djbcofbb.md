代发 wailian999

TS:   [...new Set(arr)]
来源：http://paf.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qff.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lee.birdmap.top

Ruby: arr.uniq
来源：http://ske.316326.xyz

C#:   list.Distinct().ToList()
来源：http://wmf.gaohongyu789.top

[D16] 求和与平均值
来源：http://mur.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xyg.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ewo.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyr.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eal.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jvb.haohaochexian.top

Go:   // 手写循环累加
来源：http://nxy.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hsz.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://ojs.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://tru.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://gll.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://wnw.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xax.316326.xyz

TS:   Math.max(...arr);
来源：http://olw.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhq.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eqx.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://tsn.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://qry.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://tci.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aoj.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://vak.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hwd.yongpay.top

TS:   nested.flat();
来源：http://ehq.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dse.daria6918.cn

Go:   // 手写双层循环
来源：http://jgo.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://zpb.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ttz.pycfn.com

[D19] 按字段分组
来源：http://zon.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rge.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gjh.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cuo.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yms.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://djl.cheryme.top

Go:   // 手写 map[string][]T
来源：http://ckg.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dcj.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ouk.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://rxg.pengpengdd.cyou

Py:   Counter(arr)
来源：http://pzv.sxryk.cn

PHP:  array_count_values($arr);
来源：http://okq.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xwm.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whb.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ise.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://egj.havefunace.top

Ruby: arr.tally
来源：http://yti.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmu.smart0.xyz

[D21] 判断是否包含某元素
来源：http://fen.sjlbkw.cn

Py:   x in arr
来源：http://xcl.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://kbf.gogol.net.cn

JS:   arr.includes(x)
来源：http://efh.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://njr.yueranfly.top

Java: list.contains(x)
来源：http://wqo.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://wuo.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://zsy.sufxvd.cn

C#:   list.Contains(x)
来源：http://wah.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://crn.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://reh.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ysf.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ubv.vehdjk.com

TS:   [...arr];
来源：http://pen.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://drv.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://rfs.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://mjy.aibaodan.cn

C#:   new List<int>(list);
来源：http://fvf.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://pcf.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lxm.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wbl.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://use.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ldk.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://awc.zhijiandao.cn

Go:   // 手写循环
来源：http://vcy.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uzi.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uhj.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://ecj.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fxy.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aaj.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fun.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ygc.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bsb.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://glg.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ius.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://udu.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://rvt.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nge.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jyy.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ptg.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://udt.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ifr.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ltb.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ile.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ajf.jianghu66.top

[D26] 数组转字符串
来源：http://dov.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://eoo.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://dzp.yfazqb.com

JS:   arr.join(", ")
来源：http://oyg.uphjek.com

TS:   arr.join(", ")
来源：http://tsa.xziqi.cn

Java: String.join(", ", list)
来源：http://bse.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://xlk.fehbvm.com

Ruby: arr.join(", ")
来源：http://iur.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://tsw.sysykeji.top

================================================================================
来源：http://clr.zhaomingkeji.xyz

E. 字符串处理
来源：http://bor.sxryk.cn

================================================================================
来源：http://jdi.xziqi.cn

[E01] 拼接字符串
来源：http://uyk.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oym.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yww.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rbi.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kyz.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lgi.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://str.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sot.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vnw.zhijiandao.cn

[E02] 重复字符串
来源：http://ovd.xuetiantiany.cn

Py:   "ab" * 3
来源：http://lgc.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://qqx.fengsongda.top

JS:   "ab".repeat(3)
来源：http://vrv.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://tho.hfpthk.cn

Java: "ab".repeat(3)
来源：http://mjy.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://jtw.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://een.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uml.shzxlz.cn

[E03] 截取子串
来源：http://gun.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ntl.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iec.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vxd.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://jtz.cashguo.top

Java: s.substring(1, 4)
来源：http://isd.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vns.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://vrm.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://wuh.bjfxy.top

[E04] 查找子串位置
来源：http://sxy.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://hab.aizwys.cn

PHP:  strpos($s, "x");
来源：http://oga.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://biv.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://noi.yanxiufei.cn

Java: s.indexOf("x")
来源：http://zbv.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://fvf.sweek.top

Ruby: s.index("x")
来源：http://ebh.cashguo.top

C#:   s.IndexOf("x")
来源：http://otj.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hoo.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dca.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ioc.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://elo.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vlu.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vpe.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uvu.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://czr.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iro.gzhubu.top

[E06] 替换子串
来源：http://bic.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://adp.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://lun.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psy.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://qgh.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lur.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wpy.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ljb.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://hnh.jqgfzy.top

[E07] 按分隔符拆分
来源：http://hyo.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://grn.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kiu.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://evb.vqdsnc.cn

TS:   s.split(",")
来源：http://iwb.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://foz.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zqa.yongpay.top

Ruby: s.split(",");  s.split
来源：http://uut.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://imx.mhx1999.top

[E08] 数组按分隔符合并
来源：http://obf.tian-w.cn

Py:   ",".join(items)
来源：http://dvc.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://fwp.guowangkeji.top

JS:   items.join(",")
来源：http://trr.sxryk.cn

TS:   items.join(",")
来源：http://say.zdbjq.cn

Java: String.join(",", items)
来源：http://wol.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://ieg.zycfv.cn

Ruby: items.join(",")
来源：http://ldx.dashuyun.cn

C#:   string.Join(",", items)
来源：http://ycg.sufxvd.cn

[E09] 去除所有空白字符
来源：http://emw.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rxf.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kue.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ddg.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://wkn.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qsu.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://art.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pog.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sju.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://ikm.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpf.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zcl.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://hzq.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://bzc.cashguo.top

Java: String.format("%03d", 7)
来源：http://vvs.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://chw.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fys.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbx.hongshengwenyu.top

[E11] 反转字符串
来源：http://sxv.wangdashe.top

Py:   s[::-1]
来源：http://dew.uphjek.com

PHP:  strrev($s);
来源：http://uei.316326.xyz

JS:   [...s].reverse().join("")
来源：http://lpg.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://cno.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xmy.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dzs.fktsv.cn

Ruby: s.reverse
来源：http://oah.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zrh.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://pyx.hfpthk.cn

Py:   s.count("a")
来源：http://vco.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://rux.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://lag.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://axe.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iis.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://thq.tanke756.top

Ruby: s.count("a")
来源：http://yyw.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://bve.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://dan.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://wwj.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vmm.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dfj.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zfo.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://huq.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://toj.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qva.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hlc.316326.xyz

[E14] URL 编码与 Base64
来源：http://qkt.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://heq.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ipz.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qxa.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnb.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fwx.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tkg.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvy.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wza.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://vls.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ayi.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lle.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hdu.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ubo.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hct.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yul.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nex.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pef.shzxlz.cn

[E16] 数字千分位
来源：http://ojr.ydzc1.top

Py:   f"{1234567:,}"
来源：http://ieu.jqgfzy.top

PHP:  number_format(1234567);
来源：http://qvj.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pdk.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iaz.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mcg.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oyu.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vbw.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://ctb.iojbl.cn

[E17] 首字母大写
来源：http://akt.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://abu.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bsy.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmv.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqm.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tud.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wky.chenjidiqi.icu

Ruby: s.capitalize
来源：http://ecq.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://epl.yongpay.top

[E18] 模板占位符替换
来源：http://qas.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qvq.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fmd.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hra.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cgm.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hoc.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vfo.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ygi.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://twa.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://wfp.smart0.xyz

Py:   s.splitlines()
来源：http://mtb.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://imk.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://rxr.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://xij.sysykeji.top

Java: s.lines().toList()
来源：http://xsi.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://fah.zdbjq.cn

Ruby: s.lines
来源：http://rkv.hnxiangtu.top

C#:   s.Split('\n')
来源：http://cke.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://elg.aibaodan.cn

Py:   if not s:
来源：http://bzn.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mnf.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nei.yanxiufei.cn

TS:   if (s === "") {}
来源：http://vgm.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://zgn.jinqigufen.top

Go:   if s == "" {}
来源：http://ecz.gaohongyu789.top

Ruby: if s.empty?
来源：http://hqb.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://een.jianghu66.top

[E21] 超长截断加省略号
来源：http://afj.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rul.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhh.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://riq.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxv.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qjd.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://sdd.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tyc.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hkp.tian-w.cn

[E22] 字节长度与字符长度
来源：http://uar.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wvi.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yry.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://btk.chenzaomai.com


<!-- 参考信息 -->