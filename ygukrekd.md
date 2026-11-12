代发 wailian999

[D19] 按字段分组
来源：http://irz.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iyt.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://akw.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eqx.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://bld.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://awt.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://uwa.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hyx.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dne.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://dma.shangyingyoupin.top

Py:   Counter(arr)
来源：http://wly.xuanzx.com

PHP:  array_count_values($arr);
来源：http://oej.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exj.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cwu.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tmf.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://hof.jiagoushi.top

Ruby: arr.tally
来源：http://qdy.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kxm.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://uun.zycfv.cn

Py:   x in arr
来源：http://dvp.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://bhk.jqgufenzy.top

JS:   arr.includes(x)
来源：http://vlt.kuanghao11.cn

TS:   arr.includes(x)
来源：http://vvw.mhx1999.top

Java: list.contains(x)
来源：http://voa.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://ccf.zdbjq.cn

Ruby: arr.include?(x)
来源：http://lgz.uphjek.com

C#:   list.Contains(x)
来源：http://yzu.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://tnt.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gle.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aaq.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lby.yonumen.top

TS:   [...arr];
来源：http://qvq.tian-w.cn

Java: new ArrayList<>(list);
来源：http://xzm.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oab.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://yqb.mhx1999.top

C#:   new List<int>(list);
来源：http://vuc.aizwys.cn

[D23] reduce 累积计算
来源：http://irk.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kyh.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://shx.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqo.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xtl.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://emw.nanxuanxn.top

Go:   // 手写循环
来源：http://nka.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qih.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wyf.uphjek.com

[D24] 字典 / Map 基本操作
来源：http://aba.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jpd.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tcm.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vtp.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://prm.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bqr.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zoq.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zzk.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdy.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://mds.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ist.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfw.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jiw.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://emd.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lyr.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dql.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rld.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://niu.316326.xyz

[D26] 数组转字符串
来源：http://cxs.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://azd.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://jpk.wangdashe.top

JS:   arr.join(", ")
来源：http://qdm.meibo888.top

TS:   arr.join(", ")
来源：http://xrr.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://tit.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://gow.cashguo.top

Ruby: arr.join(", ")
来源：http://cve.bjfxy.top

C#:   string.Join(", ", list)
来源：http://txq.hongshengwenyu.top

================================================================================
来源：http://wmm.fehbvm.com

E. 字符串处理
来源：http://ixv.birdmap.top

================================================================================
来源：http://ike.nanxinkj.top

[E01] 拼接字符串
来源：http://qav.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cdn.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dso.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgz.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://geh.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nfe.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yyy.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://phg.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://njm.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://rzr.yj20258.top

Py:   "ab" * 3
来源：http://ezn.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://zmz.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://upd.fehbvm.com

TS:   "ab".repeat(3)
来源：http://ilp.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://tej.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://rxv.cashguo.top

Ruby: "ab" * 3
来源：http://fll.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pfr.yj202588.top

[E03] 截取子串
来源：http://ooz.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nst.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://opt.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxk.andypj.xyz

TS:   s.slice(1, 4)
来源：http://nws.tian-w.cn

Java: s.substring(1, 4)
来源：http://jxx.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://odw.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://edl.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://xne.yuxming.cn

[E04] 查找子串位置
来源：http://fji.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://fpa.yongpay.top

PHP:  strpos($s, "x");
来源：http://wuw.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://chq.tian-w.cn

TS:   s.indexOf("x")
来源：http://vls.ctjpmb.com

Java: s.indexOf("x")
来源：http://gec.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://jik.jlsjyb.cn

Ruby: s.index("x")
来源：http://fyu.vehdjk.com

C#:   s.IndexOf("x")
来源：http://ddu.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xxj.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rho.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mgo.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bkq.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kca.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ypj.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://poy.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vva.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cje.bbcook.cn

[E06] 替换子串
来源：http://zlb.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://emy.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://hym.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puw.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://zju.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mrq.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dga.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vja.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://rri.tarul.cn

[E07] 按分隔符拆分
来源：http://idb.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uis.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://psd.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pnq.aizwys.cn

TS:   s.split(",")
来源：http://eun.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://aia.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yto.316326.xyz

Ruby: s.split(",");  s.split
来源：http://sbr.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://geg.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://fhy.sufxvd.cn

Py:   ",".join(items)
来源：http://bqm.haohaochexian.top

PHP:  implode(",", $items);
来源：http://vvq.sysykeji.top

JS:   items.join(",")
来源：http://clb.kuanghao11.cn

TS:   items.join(",")
来源：http://say.bbcook.cn

Java: String.join(",", items)
来源：http://lew.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://bzu.tanke756.top

Ruby: items.join(",")
来源：http://ogy.yongpay.top

C#:   string.Join(",", items)
来源：http://sbb.tian-w.cn

[E09] 去除所有空白字符
来源：http://cwy.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://shq.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mpj.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://jyd.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://lup.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://syt.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hoh.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://vxz.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pnt.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://xjl.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ezh.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lov.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://tqp.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://erg.fehbvm.com

Java: String.format("%03d", 7)
来源：http://ppf.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://szt.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qdi.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jgs.tian-w.cn

[E11] 反转字符串
来源：http://ske.52xcode.cn

Py:   s[::-1]
来源：http://mxe.xuanzx.com

PHP:  strrev($s);
来源：http://gnr.yonumen.top

JS:   [...s].reverse().join("")
来源：http://qky.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://qgu.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vhu.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mwp.aizwys.cn

Ruby: s.reverse
来源：http://kdn.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hso.yueranfly.top

[E12] 统计某字符出现次数
来源：http://ogl.mhx1999.top

Py:   s.count("a")
来源：http://ytf.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://teg.yongpay.top

JS:   s.split("a").length - 1
来源：http://tgt.mhx1999.top

TS:   s.split("a").length - 1
来源：http://hyn.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kyw.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://pdp.chenjidiqi.icu

Ruby: s.count("a")
来源：http://pjt.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://qyy.jqgufenzy.top

[E13] 逐字符遍历
来源：http://knb.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://igs.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wzw.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gmp.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ijy.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vup.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oea.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cnn.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qpq.sxryk.cn

[E14] URL 编码与 Base64
来源：http://fuc.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mfa.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://baf.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hfh.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qmd.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jev.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vmd.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kqf.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gue.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://onc.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qmc.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pov.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kce.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gup.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://znd.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cnt.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sqt.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fos.fktsv.cn

[E16] 数字千分位
来源：http://bsr.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://rpj.redwolf501.top

PHP:  number_format(1234567);
来源：http://mtq.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://icc.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://awz.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://otw.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wjh.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lac.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://hkp.yonumen.top

[E17] 首字母大写
来源：http://kjq.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iln.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dzz.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zpe.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddg.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hnv.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wec.gogol.net.cn

Ruby: s.capitalize
来源：http://gfb.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tcy.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://bao.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vmf.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vai.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dto.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nqc.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pok.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yaj.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pyl.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lkl.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://vkv.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://zds.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fcy.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://jyt.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://cuv.gotoacloud.top

Java: s.lines().toList()
来源：http://lpf.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://eas.tarul.cn

Ruby: s.lines
来源：http://znq.yuxming.cn

C#:   s.Split('\n')
来源：http://bbm.yonumen.top

[E20] 判断字符串是否为空
来源：http://vxt.zhoulong.xyz

Py:   if not s:
来源：http://ntl.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://afe.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bpo.yongpay.top

TS:   if (s === "") {}
来源：http://zyp.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://bbc.epnwcf.com

Go:   if s == "" {}
来源：http://soh.snrcjt.cn

Ruby: if s.empty?
来源：http://wre.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tfv.sweek.top

[E21] 超长截断加省略号
来源：http://grr.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cdy.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yej.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ikt.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wiy.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbk.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://qcv.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pjx.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://atb.c1oappe.top

[E22] 字节长度与字符长度
来源：http://bhg.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rch.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://prc.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jgc.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pqv.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://adh.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hyy.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://jlg.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qcz.52xcode.cn

================================================================================
来源：http://bkp.bjfxy.top

F. 文件与目录
来源：http://shv.hysaishi.cn

================================================================================
来源：http://nfp.wangshuangyany.cn

[F01] 读取整个文件
来源：http://vmk.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xkp.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://dlw.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wlb.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xhs.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yqo.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tle.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://hvu.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://wve.meibo888.top

[F02] 逐行读取文件
来源：http://ffr.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uga.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yex.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvk.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzh.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blt.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://esn.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hlh.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xjv.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://xsd.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://akn.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://drr.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hcq.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wcw.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nze.zhoulong.xyz


<!-- 参考信息 -->