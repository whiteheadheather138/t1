代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ldl.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://qvq.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uza.birdmap.top

TS:   nested.flat();
来源：http://ono.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xon.yuxming.cn

Go:   // 手写双层循环
来源：http://hin.tarul.cn

Ruby: nested.flatten
来源：http://pmw.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vhd.fehbvm.com

[D19] 按字段分组
来源：http://lyd.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbp.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eim.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yee.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jzp.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sny.havefunace.top

Go:   // 手写 map[string][]T
来源：http://pem.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aqc.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ejf.ivvv.top

[D20] 统计每个元素出现次数
来源：http://rsm.shangyingyoupin.top

Py:   Counter(arr)
来源：http://lsk.nwbrower.top

PHP:  array_count_values($arr);
来源：http://wpk.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdz.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eik.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hli.52xcode.cn

Go:   // 手写 map[T]int
来源：http://zwv.fzhhl.top

Ruby: arr.tally
来源：http://lpt.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yay.gzhubu.top

[D21] 判断是否包含某元素
来源：http://ane.ivvv.top

Py:   x in arr
来源：http://hmi.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://ysr.yanxiufei.cn

JS:   arr.includes(x)
来源：http://gon.daria6918.cn

TS:   arr.includes(x)
来源：http://htg.xylfe.cn

Java: list.contains(x)
来源：http://ems.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://uth.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://jjv.52xcode.cn

C#:   list.Contains(x)
来源：http://qtq.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://wze.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sjm.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://shw.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://umg.0kj1m.cn

TS:   [...arr];
来源：http://cfe.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://yhv.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vmu.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://efr.chenlongwang.top

C#:   new List<int>(list);
来源：http://lid.iojbl.cn

[D23] reduce 累积计算
来源：http://cfj.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yng.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ccl.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awy.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ivp.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zda.tian-w.cn

Go:   // 手写循环
来源：http://zms.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cci.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cyq.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://azv.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://grk.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ssn.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qvn.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://peh.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kfx.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tmj.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cim.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nyc.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://hey.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://brq.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qlb.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xge.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dpe.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://scr.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rdd.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jik.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qom.yongpay.top

[D26] 数组转字符串
来源：http://qks.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://juv.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://geq.daria6918.cn

JS:   arr.join(", ")
来源：http://hpl.tarul.cn

TS:   arr.join(", ")
来源：http://srz.ydzc1.top

Java: String.join(", ", list)
来源：http://bgf.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://ioe.hnqzz.top

Ruby: arr.join(", ")
来源：http://cxj.xylfe.cn

C#:   string.Join(", ", list)
来源：http://msv.tian-w.cn

================================================================================
来源：http://hto.ywan-chungtsiang.top

E. 字符串处理
来源：http://bxv.shzxlz.cn

================================================================================
来源：http://iiw.316326.xyz

[E01] 拼接字符串
来源：http://nsx.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://url.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jrl.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjc.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://prf.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dvc.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iyc.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtd.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://upy.aibaodan.cn

[E02] 重复字符串
来源：http://cum.sxryk.cn

Py:   "ab" * 3
来源：http://mqb.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://iua.hesvh.cn

JS:   "ab".repeat(3)
来源：http://jgv.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://mpw.ydzc1.top

Java: "ab".repeat(3)
来源：http://cfu.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://pqy.ydjk.org.cn

Ruby: "ab" * 3
来源：http://flv.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pye.quarkkingdee.top

[E03] 截取子串
来源：http://hef.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nsv.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwf.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xfp.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://zqu.uphjek.com

Java: s.substring(1, 4)
来源：http://vwq.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jdw.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wtr.yj202588.top

C#:   s.Substring(1, 3)
来源：http://yzm.jlsjyb.cn

[E04] 查找子串位置
来源：http://sad.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://eco.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://nzk.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jdh.xinyue.icu

TS:   s.indexOf("x")
来源：http://gmj.quarkkingdee.top

Java: s.indexOf("x")
来源：http://rbw.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://tvf.gotoacloud.top

Ruby: s.index("x")
来源：http://sem.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://fli.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kly.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uiv.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xii.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gbv.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jfc.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qaq.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zya.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xea.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vlz.52xcode.cn

[E06] 替换子串
来源：http://nbv.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hlf.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://nhh.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vqb.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://jgu.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ony.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qyk.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aft.yonumen.top

C#:   s.Replace("a", "b")
来源：http://imf.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://ert.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajd.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://btn.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hzd.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://vpq.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://hcu.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qpw.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://fmr.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://woy.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://xpi.xuanzx.com

Py:   ",".join(items)
来源：http://ims.redwolf501.top

PHP:  implode(",", $items);
来源：http://gwr.jqgufenzy.top

JS:   items.join(",")
来源：http://aal.jyoumei.cn

TS:   items.join(",")
来源：http://ykr.haohaochexian.top

Java: String.join(",", items)
来源：http://ltk.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://qif.cheryme.top

Ruby: items.join(",")
来源：http://dgj.cdnleiting.top

C#:   string.Join(",", items)
来源：http://ncw.yvedp.cn

[E09] 去除所有空白字符
来源：http://vcr.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yxq.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfl.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://erk.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://jny.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://apn.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://unx.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://jdb.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vya.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://hxq.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rqg.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jho.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://hov.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://uut.redwolf501.top

Java: String.format("%03d", 7)
来源：http://lal.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bkp.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oiq.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bri.hesvh.cn

[E11] 反转字符串
来源：http://rrn.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://bde.xuanzx.com

PHP:  strrev($s);
来源：http://sek.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://mxk.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://gvb.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://osb.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jqd.sweek.top

Ruby: s.reverse
来源：http://ayv.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ifg.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://euv.zhiwuduotai.top

Py:   s.count("a")
来源：http://dcf.meibo888.top

PHP:  substr_count($s, "a");
来源：http://isk.xziqi.cn

JS:   s.split("a").length - 1
来源：http://enu.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://ypz.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uzf.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://jbs.birdmap.top

Ruby: s.count("a")
来源：http://qnn.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://vjc.kuanghao11.cn

[E13] 逐字符遍历
来源：http://mmx.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://cph.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mep.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwi.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://tht.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ela.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qru.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://unj.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nys.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://jrv.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pkq.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vys.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucp.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rwp.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jjh.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jtc.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qak.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lgh.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://pnc.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iyz.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lqp.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://auu.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lqv.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ohz.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yia.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cim.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://til.ybcxt.top

[E16] 数字千分位
来源：http://phb.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://qpo.guannengcc.top

PHP:  number_format(1234567);
来源：http://woo.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dsd.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ujy.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fey.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://znj.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://evq.uphjek.com

C#:   1234567.ToString("N0")
来源：http://ueg.haohaochexian.top

[E17] 首字母大写
来源：http://eip.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fmw.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tba.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oki.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbp.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jut.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dgv.tarul.cn

Ruby: s.capitalize
来源：http://khr.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ift.zhixingplan.top

[E18] 模板占位符替换
来源：http://dxn.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zvn.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://owz.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mmc.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tzk.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bkv.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kbd.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlp.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ikc.pycfn.com

[E19] 多行文本按行拆分
来源：http://ynd.bbcook.cn

Py:   s.splitlines()
来源：http://ach.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wlq.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://nzf.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://gcj.chenzaomai.com

Java: s.lines().toList()
来源：http://pnt.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://fct.ydzc1.top

Ruby: s.lines
来源：http://yav.yueranfly.top

C#:   s.Split('\n')
来源：http://lzy.pycfn.com

[E20] 判断字符串是否为空
来源：http://umq.nanxinkj.top

Py:   if not s:
来源：http://jei.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yrz.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lpd.birdmap.top

TS:   if (s === "") {}
来源：http://fwq.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://mxa.daria6918.cn

Go:   if s == "" {}
来源：http://wpt.sweek.top

Ruby: if s.empty?
来源：http://usx.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sof.daria6918.cn

[E21] 超长截断加省略号
来源：http://yiw.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://woh.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bfq.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cio.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wux.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://idv.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://tdt.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yol.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sce.yj20258.top

[E22] 字节长度与字符长度
来源：http://hbx.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvy.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvp.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ram.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aku.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zbl.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eai.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://dix.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://upc.gaohongyu789.top

================================================================================
来源：http://pwx.jqgufenzy.top

F. 文件与目录
来源：http://kyb.ppjwa.cn

================================================================================
来源：http://uft.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://rqk.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ylf.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://hwz.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://syj.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://otk.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://efy.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://apx.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://qjv.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://mby.vqdsnc.cn

[F02] 逐行读取文件
来源：http://xgh.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oxq.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ntt.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fgu.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edq.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tko.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jvj.ybcxt.top


<!-- 参考信息 -->