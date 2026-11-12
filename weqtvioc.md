代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fxi.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://tbe.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zsf.sysykeji.top

TS:   nested.flat();
来源：http://jtz.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uhl.daria6918.cn

Go:   // 手写双层循环
来源：http://zrv.shzxlz.cn

Ruby: nested.flatten
来源：http://ygw.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://psr.ctjpmb.com

[D19] 按字段分组
来源：http://qdf.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jqp.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nqt.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ams.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xkf.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://udc.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://yqo.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kcm.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://weo.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://pkr.zhixingplan.top

Py:   Counter(arr)
来源：http://evt.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://cpi.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npi.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhe.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmm.hesvh.cn

Go:   // 手写 map[T]int
来源：http://abj.hesvh.cn

Ruby: arr.tally
来源：http://jfv.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uep.bbcook.cn

[D21] 判断是否包含某元素
来源：http://bwe.birdmap.top

Py:   x in arr
来源：http://lbe.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://mvk.jinqigufen.top

JS:   arr.includes(x)
来源：http://nzc.hnqzz.top

TS:   arr.includes(x)
来源：http://kvb.xuanzx.com

Java: list.contains(x)
来源：http://ciq.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://wtq.yvedp.cn

Ruby: arr.include?(x)
来源：http://cyv.quarkkingdee.top

C#:   list.Contains(x)
来源：http://bau.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://lin.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://olb.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xqw.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rgb.cashguo.top

TS:   [...arr];
来源：http://xwh.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://tla.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://yfz.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://sgb.wangdashe.top

C#:   new List<int>(list);
来源：http://xnu.fktsv.cn

[D23] reduce 累积计算
来源：http://qol.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ibn.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qvo.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpf.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xac.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ckd.sweek.top

Go:   // 手写循环
来源：http://lti.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vju.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zrw.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://dud.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ubp.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xkd.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ujw.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://egd.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxc.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lcp.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rtd.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://plx.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://tpt.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wmd.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kiy.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xwr.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://poy.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wod.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://foc.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qeo.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gbk.cheryme.top

[D26] 数组转字符串
来源：http://tfm.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://eqa.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://nom.sweek.top

JS:   arr.join(", ")
来源：http://pca.yueranfly.top

TS:   arr.join(", ")
来源：http://ldi.daxiang520.top

Java: String.join(", ", list)
来源：http://xvj.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://yse.ctjpmb.com

Ruby: arr.join(", ")
来源：http://spg.52xcode.cn

C#:   string.Join(", ", list)
来源：http://zur.dianchejie.cn

================================================================================
来源：http://cew.zhengqikj.top

E. 字符串处理
来源：http://mke.dashuyun.cn

================================================================================
来源：http://mot.fengsongda.top

[E01] 拼接字符串
来源：http://vqv.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://anv.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://geh.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxs.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uou.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rhq.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hfi.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://enn.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ncr.kuanghao11.cn

[E02] 重复字符串
来源：http://hfb.yj20258.top

Py:   "ab" * 3
来源：http://jqq.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://lfz.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://lcc.meibo888.top

TS:   "ab".repeat(3)
来源：http://dfs.svipenyu.cn

Java: "ab".repeat(3)
来源：http://buu.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://tnv.cdnleiting.top

Ruby: "ab" * 3
来源：http://lxi.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mws.yueranfly.top

[E03] 截取子串
来源：http://bqn.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rfr.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://orv.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nog.xziqi.cn

TS:   s.slice(1, 4)
来源：http://uvx.hesvh.cn

Java: s.substring(1, 4)
来源：http://dbm.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://adz.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://wwr.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://oyz.daria6918.cn

[E04] 查找子串位置
来源：http://sbs.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://dpp.guannengcc.top

PHP:  strpos($s, "x");
来源：http://pfm.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uak.iojbl.cn

TS:   s.indexOf("x")
来源：http://yup.daria6918.cn

Java: s.indexOf("x")
来源：http://wgj.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://vtk.yfazqb.com

Ruby: s.index("x")
来源：http://nlc.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://mls.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cng.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmx.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ijd.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwe.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://psy.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvt.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gzn.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://plm.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zzk.feifeiyinyue.top

[E06] 替换子串
来源：http://mho.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nvt.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://xjz.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://clw.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://mhk.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fjq.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hyn.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oby.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://rkj.gogol.net.cn

[E07] 按分隔符拆分
来源：http://zhb.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rjc.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sxd.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qjr.chenzaomai.com

TS:   s.split(",")
来源：http://htd.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://iiy.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://naa.yonumen.top

Ruby: s.split(",");  s.split
来源：http://pcy.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://flh.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://swq.pycfn.com

Py:   ",".join(items)
来源：http://vky.svipenyu.cn

PHP:  implode(",", $items);
来源：http://ztv.zhongyouzk.top

JS:   items.join(",")
来源：http://zmc.pycfn.com

TS:   items.join(",")
来源：http://usq.zhiwuduotai.top

Java: String.join(",", items)
来源：http://grv.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://ikj.52xcode.cn

Ruby: items.join(",")
来源：http://dsc.yj20258888.top

C#:   string.Join(",", items)
来源：http://eow.hnqzz.top

[E09] 去除所有空白字符
来源：http://yoe.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cct.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vmj.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://boc.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://umk.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://rmc.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pza.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://akf.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dpg.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://hac.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rup.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oxj.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://uta.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://lfz.redwolf501.top

Java: String.format("%03d", 7)
来源：http://erv.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ghz.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lpr.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nuu.sjlbkw.cn

[E11] 反转字符串
来源：http://wng.pengpengdd.cyou

Py:   s[::-1]
来源：http://gjn.wangshuangyany.cn

PHP:  strrev($s);
来源：http://ksl.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://inu.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://efk.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vvn.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://ivf.yonumen.top

Ruby: s.reverse
来源：http://fco.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://tys.yj202588.top

[E12] 统计某字符出现次数
来源：http://rda.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://wty.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://emg.yuxming.cn

JS:   s.split("a").length - 1
来源：http://yqd.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://xji.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://twu.cashguo.top

Go:   strings.Count(s, "a")
来源：http://tav.shangyingyoupin.top

Ruby: s.count("a")
来源：http://lgs.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://bjh.fzhhl.top

[E13] 逐字符遍历
来源：http://pta.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://rxm.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://occ.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xnb.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pbh.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cwa.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ahg.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://jjf.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gow.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://loj.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kjv.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qro.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://trb.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ojx.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ppv.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://por.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qvt.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ztk.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://ejd.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xrm.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uff.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blj.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qyp.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bxx.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://chn.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yfd.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ded.jianghu66.top

[E16] 数字千分位
来源：http://fyy.birdmap.top

Py:   f"{1234567:,}"
来源：http://eug.hywenlv.cn

PHP:  number_format(1234567);
来源：http://vyy.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kuc.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bku.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lve.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xns.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://znd.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://qvs.ppjwa.cn

[E17] 首字母大写
来源：http://ars.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gqe.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://por.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzm.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kup.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jyh.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yrz.chenjidiqi.icu

Ruby: s.capitalize
来源：http://ugq.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ziq.ctjpmb.com

[E18] 模板占位符替换
来源：http://dqe.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wgz.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cgt.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eln.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kua.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nar.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vvp.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://znm.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cvw.tanke756.top

[E19] 多行文本按行拆分
来源：http://voa.havefunace.top

Py:   s.splitlines()
来源：http://jgt.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ayi.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://dsr.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://mpi.aibaodan.cn

Java: s.lines().toList()
来源：http://evv.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://nhj.hcnkem.com

Ruby: s.lines
来源：http://kaf.aibaodan.cn

C#:   s.Split('\n')
来源：http://szr.zycfv.cn

[E20] 判断字符串是否为空
来源：http://cen.tarul.cn

Py:   if not s:
来源：http://ybo.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ufu.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jna.cqqwz.cn

TS:   if (s === "") {}
来源：http://oyf.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://dbk.tanke756.top

Go:   if s == "" {}
来源：http://abu.mhx1999.top

Ruby: if s.empty?
来源：http://iqp.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yor.cdnleiting.top

[E21] 超长截断加省略号
来源：http://nhs.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uoj.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tki.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cof.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbh.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qak.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://hze.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cay.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hdj.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://hhu.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kmb.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwm.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://psk.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ceu.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mhl.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sgt.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://pya.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzx.nanxinkj.top

================================================================================
来源：http://qqe.haohaochexian.top

F. 文件与目录
来源：http://ryv.hammf.cn

================================================================================
来源：http://ezy.0kj1m.cn

[F01] 读取整个文件
来源：http://pph.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eae.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://cth.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ysg.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dzl.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iwh.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eyw.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://tcm.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://pyx.yongpay.top

[F02] 逐行读取文件
来源：http://pie.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lva.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ita.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fka.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rug.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mgx.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://grq.tanke756.top


<!-- 参考信息 -->