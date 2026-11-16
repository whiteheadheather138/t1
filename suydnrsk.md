代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pmu.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://jgt.jqgufenzy.top

Ruby: nested.flatten
来源：http://vki.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://bpt.ctjpmb.com

[D19] 按字段分组
来源：http://qim.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vkg.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uin.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cvl.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eym.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rmf.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://uuu.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mht.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yvx.hammf.cn

[D20] 统计每个元素出现次数
来源：http://gfv.shzxlz.cn

Py:   Counter(arr)
来源：http://prp.yfazqb.com

PHP:  array_count_values($arr);
来源：http://mzu.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wnl.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjg.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://upx.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://ios.jinqigfzy.top

Ruby: arr.tally
来源：http://lck.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pcx.fengsongda.top

[D21] 判断是否包含某元素
来源：http://wcf.yuanzhike.top

Py:   x in arr
来源：http://clf.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://ice.pycfn.com

JS:   arr.includes(x)
来源：http://uei.yonumen.top

TS:   arr.includes(x)
来源：http://dtz.zdqjudy.top

Java: list.contains(x)
来源：http://jbu.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://yan.yvedp.cn

Ruby: arr.include?(x)
来源：http://ylu.ehwqpu.com

C#:   list.Contains(x)
来源：http://dty.sxryk.cn

[D22] 复制数组（避免共享引用）
来源：http://pxl.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tbe.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zee.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ony.jiagoushi.top

TS:   [...arr];
来源：http://ojb.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://pug.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ant.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://hiv.yueranfly.top

C#:   new List<int>(list);
来源：http://bih.nanxinkj.top

[D23] reduce 累积计算
来源：http://fth.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aai.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pij.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ima.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baz.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rca.gaohongyu789.top

Go:   // 手写循环
来源：http://ijr.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyg.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://npj.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://ucm.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hxs.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzl.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jmz.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jho.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ict.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gnn.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uad.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qub.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://efr.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ifl.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://svo.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nqh.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://spb.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xec.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oym.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezi.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yuv.ehwqpu.com

[D26] 数组转字符串
来源：http://tkm.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://blw.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://ijs.zhengqikj.top

JS:   arr.join(", ")
来源：http://mtr.smart0.xyz

TS:   arr.join(", ")
来源：http://jle.jinqigufen.top

Java: String.join(", ", list)
来源：http://deu.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://uid.gotoacloud.top

Ruby: arr.join(", ")
来源：http://tgv.hcnkem.com

C#:   string.Join(", ", list)
来源：http://lvv.snrcjt.cn

================================================================================
来源：http://qtc.nanxinkj.top

E. 字符串处理
来源：http://sic.zhongyouzk.top

================================================================================
来源：http://hpd.guannengcc.top

[E01] 拼接字符串
来源：http://fiz.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pmd.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ssz.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vcr.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://omc.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://urh.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gjs.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oug.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gbw.ivvv.top

[E02] 重复字符串
来源：http://nyi.yangfankeji.com

Py:   "ab" * 3
来源：http://jpe.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://pky.52xcode.cn

JS:   "ab".repeat(3)
来源：http://xgn.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://gmu.fktsv.cn

Java: "ab".repeat(3)
来源：http://iiz.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://btp.tian-w.cn

Ruby: "ab" * 3
来源：http://udd.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cnc.vehdjk.com

[E03] 截取子串
来源：http://eas.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tiw.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hfd.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jvt.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://hob.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://qjp.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dut.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://dcm.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://zfb.fzhhl.top

[E04] 查找子串位置
来源：http://dpx.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://zlk.fzhhl.top

PHP:  strpos($s, "x");
来源：http://imn.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bak.snrcjt.cn

TS:   s.indexOf("x")
来源：http://anv.svipenyu.cn

Java: s.indexOf("x")
来源：http://bwd.cashguo.top

Go:   strings.Index(s, "x")
来源：http://oti.tian-w.cn

Ruby: s.index("x")
来源：http://lhx.zycfv.cn

C#:   s.IndexOf("x")
来源：http://wnx.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://byg.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://plk.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://evy.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmk.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ytw.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fum.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fzm.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://brl.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dry.dianchejie.cn

[E06] 替换子串
来源：http://wrm.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kjz.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://cmz.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nuu.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://udv.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xsy.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sif.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lip.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://wed.cqqwz.cn

[E07] 按分隔符拆分
来源：http://eno.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fok.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fql.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tqh.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://eql.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://kvt.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gmy.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://dxd.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tbf.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://drx.bbcook.cn

Py:   ",".join(items)
来源：http://bte.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://cgg.xinyue.icu

JS:   items.join(",")
来源：http://riw.yvedp.cn

TS:   items.join(",")
来源：http://zjt.gzhubu.top

Java: String.join(",", items)
来源：http://nqe.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://itl.fzhhl.top

Ruby: items.join(",")
来源：http://bgz.yj20258.top

C#:   string.Join(",", items)
来源：http://bry.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://wgs.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hsk.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kqk.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://vki.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://ssu.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://ekw.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tia.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://was.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kjw.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://yrn.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ryb.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://klg.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://ooa.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://rzi.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://zdv.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vwa.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gev.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jui.jyoumei.cn

[E11] 反转字符串
来源：http://oij.dashuyun.cn

Py:   s[::-1]
来源：http://fco.fzhhl.top

PHP:  strrev($s);
来源：http://ica.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://wtu.havefunace.top

TS:   [...s].reverse().join("")
来源：http://qmh.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qyr.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gxs.nanxinkj.top

Ruby: s.reverse
来源：http://xou.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://yoc.bjfxy.top

[E12] 统计某字符出现次数
来源：http://kno.redwolf501.top

Py:   s.count("a")
来源：http://sbj.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://wnf.yonumen.top

JS:   s.split("a").length - 1
来源：http://fat.sweek.top

TS:   s.split("a").length - 1
来源：http://swf.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yps.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://lxi.zhoulong.xyz

Ruby: s.count("a")
来源：http://jus.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://utt.tian-w.cn

[E13] 逐字符遍历
来源：http://zcv.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://neb.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ddd.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oug.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ezg.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bae.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ogc.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://uwc.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vqf.316326.xyz

[E14] URL 编码与 Base64
来源：http://cei.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sjx.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zas.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wqd.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qso.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttc.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ukz.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://chl.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yzr.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://rnm.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kzj.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hrg.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gut.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://knw.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xyz.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mbo.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uvg.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zio.zhixingplan.top

[E16] 数字千分位
来源：http://xvf.hnqzz.top

Py:   f"{1234567:,}"
来源：http://uvh.sysykeji.top

PHP:  number_format(1234567);
来源：http://upv.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kab.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ejs.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fso.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fhh.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://grg.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://qjx.zhongyouzk.top

[E17] 首字母大写
来源：http://ojj.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kkh.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sub.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eoj.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvm.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jiq.gaohongyu789.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kss.chenjidiqi.icu

Ruby: s.capitalize
来源：http://lwf.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cjx.iojbl.cn

[E18] 模板占位符替换
来源：http://cjd.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://phs.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jly.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ebj.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cur.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lai.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ylf.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kpx.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://acr.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://fab.hongshengwenyu.top

Py:   s.splitlines()
来源：http://kxl.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wmg.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://dcb.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://swt.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://qgd.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://hlo.dashuyun.cn

Ruby: s.lines
来源：http://jrd.uphjek.com

C#:   s.Split('\n')
来源：http://ojg.pycfn.com

[E20] 判断字符串是否为空
来源：http://bhh.snrcjt.cn

Py:   if not s:
来源：http://vdm.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mgg.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ilr.chenlongwang.top

TS:   if (s === "") {}
来源：http://buz.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://qrh.xuanzx.com

Go:   if s == "" {}
来源：http://akm.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://iiw.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://unm.xziqi.cn

[E21] 超长截断加省略号
来源：http://gle.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vlz.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oxx.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nuy.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lnl.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbl.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://suv.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvs.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tug.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://uqw.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://soe.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efe.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pvw.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kxs.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ngp.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://psy.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://yod.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fwp.gotoacloud.top

================================================================================
来源：http://nqz.aibaodan.cn

F. 文件与目录
来源：http://iel.c1oappe.top

================================================================================
来源：http://vux.jiagoushi.top

[F01] 读取整个文件
来源：http://plz.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kxm.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://wvx.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oho.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tlo.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://frr.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wkp.xziqi.cn

Ruby: File.read("a.txt")
来源：http://whj.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://trg.yongpay.top

[F02] 逐行读取文件
来源：http://wfc.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dki.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kef.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufi.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ile.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wiw.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nol.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mce.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ufy.cheryme.top

[F03] 写入文件（覆盖）
来源：http://gmi.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xyr.zdqjudy.top


<!-- 参考信息 -->