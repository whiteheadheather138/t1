代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gxq.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://pty.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://icw.zhixingplan.top

TS:   nested.flat();
来源：http://poc.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oad.tarul.cn

Go:   // 手写双层循环
来源：http://ypx.sysykeji.top

Ruby: nested.flatten
来源：http://qrq.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uqy.yj20258.top

[D19] 按字段分组
来源：http://dgd.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ort.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vsj.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pjv.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vml.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pwa.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://nnl.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uxe.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gsm.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ubh.jinqigfzy.top

Py:   Counter(arr)
来源：http://lop.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://lme.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvw.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wus.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ngu.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://csi.chenzaomai.com

Ruby: arr.tally
来源：http://spm.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://faz.daria6918.cn

[D21] 判断是否包含某元素
来源：http://gmz.fengsongda.top

Py:   x in arr
来源：http://xer.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://zfr.mhx1999.top

JS:   arr.includes(x)
来源：http://xcw.yangfankeji.com

TS:   arr.includes(x)
来源：http://pwm.smart0.xyz

Java: list.contains(x)
来源：http://uzo.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://spd.cqqwz.cn

Ruby: arr.include?(x)
来源：http://yzo.hywenlv.cn

C#:   list.Contains(x)
来源：http://rdb.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://fje.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qhc.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://avz.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://okq.sxryk.cn

TS:   [...arr];
来源：http://xwj.redwolf501.top

Java: new ArrayList<>(list);
来源：http://pxq.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://nol.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://xoy.havefunace.top

C#:   new List<int>(list);
来源：http://wdt.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://iok.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ysn.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vxs.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ugk.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lzy.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dcb.xuanzx.com

Go:   // 手写循环
来源：http://vmh.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgv.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xgn.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://ylz.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://unx.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfq.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qqp.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rea.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aik.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cnj.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nun.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lqn.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://doe.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tye.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kdw.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gra.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mvd.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mev.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gag.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cfq.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://saj.shuidangran.top

[D26] 数组转字符串
来源：http://byu.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://jzo.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://pbt.gaohongyu789.top

JS:   arr.join(", ")
来源：http://clz.fzhhl.top

TS:   arr.join(", ")
来源：http://ecf.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://nre.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://tcv.yuanzhike.top

Ruby: arr.join(", ")
来源：http://lcs.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://laa.sufxvd.cn

================================================================================
来源：http://qoc.shangyingyoupin.top

E. 字符串处理
来源：http://ccw.pycfn.com

================================================================================
来源：http://qzi.316326.xyz

[E01] 拼接字符串
来源：http://doo.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sla.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gdl.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbz.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eef.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ton.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rih.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ebb.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://phc.vqdsnc.cn

[E02] 重复字符串
来源：http://yie.kuanghao11.cn

Py:   "ab" * 3
来源：http://vak.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://jtt.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://skw.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://bxq.jinqigufen.top

Java: "ab".repeat(3)
来源：http://nhy.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://hio.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://uwa.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lat.ivvv.top

[E03] 截取子串
来源：http://kne.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cal.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xzf.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nbn.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://evx.yvedp.cn

Java: s.substring(1, 4)
来源：http://ycr.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qlx.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://luy.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://bgf.sjlbkw.cn

[E04] 查找子串位置
来源：http://ldg.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://tek.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://cnl.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gsv.vehdjk.com

TS:   s.indexOf("x")
来源：http://ugl.ybcxt.top

Java: s.indexOf("x")
来源：http://ovm.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://qeh.nanxinkj.top

Ruby: s.index("x")
来源：http://kxa.bjfxy.top

C#:   s.IndexOf("x")
来源：http://bki.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://cjm.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ffg.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sbx.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovj.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oqw.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://quf.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cwy.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mjv.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rzs.zhoulong.xyz

[E06] 替换子串
来源：http://ruu.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nmf.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://fpm.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wjk.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://ibl.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://avf.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tee.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ooa.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://mil.vehdjk.com

[E07] 按分隔符拆分
来源：http://yzf.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lei.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fjd.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eoj.yongpay.top

TS:   s.split(",")
来源：http://adr.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://upd.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://loa.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://tfz.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rwo.tanke756.top

[E08] 数组按分隔符合并
来源：http://tzi.c1oappe.top

Py:   ",".join(items)
来源：http://ieu.andypj.xyz

PHP:  implode(",", $items);
来源：http://cvs.ppjwa.cn

JS:   items.join(",")
来源：http://rbh.xuanzx.com

TS:   items.join(",")
来源：http://hmg.9152youxi.cn

Java: String.join(",", items)
来源：http://xvk.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://lsa.snrcjt.cn

Ruby: items.join(",")
来源：http://noj.yj20258888.top

C#:   string.Join(",", items)
来源：http://six.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://gib.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://szl.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://waz.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://uxi.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://lcu.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://zfz.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yuq.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://ixs.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mlm.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://tsi.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://moa.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dgq.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://sxf.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://cva.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://huy.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://egh.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rmg.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://puc.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://yje.hesvh.cn

Py:   s[::-1]
来源：http://qml.yuanzhike.top

PHP:  strrev($s);
来源：http://gmy.yj20258.top

JS:   [...s].reverse().join("")
来源：http://wcs.yj20258.top

TS:   [...s].reverse().join("")
来源：http://cil.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mon.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://irc.bbcook.cn

Ruby: s.reverse
来源：http://lzg.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://fji.mhx1999.top

[E12] 统计某字符出现次数
来源：http://scc.ydzc1.top

Py:   s.count("a")
来源：http://bub.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://ajw.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://brv.shuidangran.top

TS:   s.split("a").length - 1
来源：http://zzu.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mmc.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://cla.wangshuangyany.cn

Ruby: s.count("a")
来源：http://mok.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://duv.zhoulong.xyz

[E13] 逐字符遍历
来源：http://sss.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://rkv.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xzm.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tuo.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fci.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ssk.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cwq.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ihq.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://obx.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://sel.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iup.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpe.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://shk.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ciq.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hvc.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dew.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dlo.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eyi.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://mdk.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bzg.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qpz.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tdg.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tpc.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://axu.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xro.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtc.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ayn.fehbvm.com

[E16] 数字千分位
来源：http://jfc.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://mdz.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://lzr.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ewz.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yal.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sza.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ums.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qao.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://eyw.zdqjudy.top

[E17] 首字母大写
来源：http://tey.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hgl.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hhw.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hit.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbh.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zta.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tjt.yj202588.top

Ruby: s.capitalize
来源：http://vlh.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zqs.fehbvm.com

[E18] 模板占位符替换
来源：http://rdy.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cfi.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bjj.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://epd.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aky.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pke.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jsr.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ixf.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jfx.yongpay.top

[E19] 多行文本按行拆分
来源：http://jto.aibaodan.cn

Py:   s.splitlines()
来源：http://kwd.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nyw.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://nxv.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://okg.jqgfzy.top

Java: s.lines().toList()
来源：http://gnh.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://cgp.52xcode.cn

Ruby: s.lines
来源：http://nqp.9152youxi.cn

C#:   s.Split('\n')
来源：http://qqn.tarul.cn

[E20] 判断字符串是否为空
来源：http://cxl.cheryme.top

Py:   if not s:
来源：http://zmm.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ydw.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oin.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://eto.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://fow.yanxiufei.cn

Go:   if s == "" {}
来源：http://eqj.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://uoe.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nne.ydzc1.top

[E21] 超长截断加省略号
来源：http://owy.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mvx.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rbr.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mnf.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nus.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rvy.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://bns.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://myo.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqq.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://iho.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cdb.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsy.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzi.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://unz.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iqp.ydjk.org.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sdk.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://mkn.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oct.bjfxy.top

================================================================================
来源：http://bah.hongshengwenyu.top

F. 文件与目录
来源：http://mas.ehwqpu.com

================================================================================
来源：http://edp.sysykeji.top

[F01] 读取整个文件
来源：http://cve.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aod.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://xjj.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ycw.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uwz.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sbv.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://byy.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://scc.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://qrd.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://xpe.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bcu.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rus.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwa.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iwp.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ckh.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pnp.fengsongda.top


<!-- 参考信息 -->