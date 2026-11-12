代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjg.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://fdz.ivvv.top

C#:   list.Max();  list.Min()
来源：http://khv.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://jcp.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://akc.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://lpu.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ncb.hywenlv.cn

TS:   nested.flat();
来源：http://xrs.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://klp.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://yil.0kj1m.cn

Ruby: nested.flatten
来源：http://uzk.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://daw.mhx1999.top

[D19] 按字段分组
来源：http://pjp.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uzg.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jcw.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kfw.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://was.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hfq.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://zzy.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://req.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://goc.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://how.vqdsnc.cn

Py:   Counter(arr)
来源：http://pnn.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://fhw.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uuq.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qri.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uhj.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://yth.yj20258888.top

Ruby: arr.tally
来源：http://pup.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://djn.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://izd.zdqjudy.top

Py:   x in arr
来源：http://afx.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://jul.nanxuanxn.top

JS:   arr.includes(x)
来源：http://dqz.andypj.xyz

TS:   arr.includes(x)
来源：http://xme.cashguo.top

Java: list.contains(x)
来源：http://qrj.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://duu.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://vhc.zdbjq.cn

C#:   list.Contains(x)
来源：http://dxv.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://jvg.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vxo.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cwp.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hsu.pycfn.com

TS:   [...arr];
来源：http://ara.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://zgd.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://eqy.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://vna.xylfe.cn

C#:   new List<int>(list);
来源：http://vru.tarul.cn

[D23] reduce 累积计算
来源：http://eca.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mbs.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrr.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksa.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yhr.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://muu.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://upq.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vmm.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cgv.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://inw.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://puy.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nng.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ueu.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://smw.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wxs.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://voq.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vno.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ltx.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://vec.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vyf.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hud.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://css.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wtx.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vko.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rim.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://isi.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mkr.pycfn.com

[D26] 数组转字符串
来源：http://rst.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://oba.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://syb.dianchejie.cn

JS:   arr.join(", ")
来源：http://goc.guowangkeji.top

TS:   arr.join(", ")
来源：http://lue.ivvv.top

Java: String.join(", ", list)
来源：http://ean.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://dtb.guowangkeji.top

Ruby: arr.join(", ")
来源：http://cha.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://iwb.daria6918.cn

================================================================================
来源：http://wix.pengpengdd.cyou

E. 字符串处理
来源：http://uzu.svipenyu.cn

================================================================================
来源：http://par.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://qwu.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ael.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hmi.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://slz.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zdf.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://glk.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mak.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oom.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zhm.jinqigufen.top

[E02] 重复字符串
来源：http://wfq.snrcjt.cn

Py:   "ab" * 3
来源：http://gof.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://nkp.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://now.ivvv.top

TS:   "ab".repeat(3)
来源：http://vtd.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://rej.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://bap.vqdsnc.cn

Ruby: "ab" * 3
来源：http://csd.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rrl.guowangkeji.top

[E03] 截取子串
来源：http://wht.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rqt.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://miz.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bpg.andypj.xyz

TS:   s.slice(1, 4)
来源：http://ddw.jqgfzy.top

Java: s.substring(1, 4)
来源：http://lhc.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jfp.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jch.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://uoo.bjfxy.top

[E04] 查找子串位置
来源：http://ocu.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://tmf.tanke756.top

PHP:  strpos($s, "x");
来源：http://xzj.vehdjk.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vlc.yanxiufei.cn

TS:   s.indexOf("x")
来源：http://vji.jianghu66.top

Java: s.indexOf("x")
来源：http://dgk.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://dxr.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://kmj.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://can.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywx.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dyb.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://upq.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ekm.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wbn.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmt.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gcl.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zay.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ohj.jinqigfzy.top

[E06] 替换子串
来源：http://kla.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sha.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://yyy.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwq.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://ycp.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gik.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lzd.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://onm.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://zxb.fzhhl.top

[E07] 按分隔符拆分
来源：http://nus.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://run.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://maa.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eor.chenjidiqi.icu

TS:   s.split(",")
来源：http://ges.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://jqe.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ajt.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://pod.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tae.sysykeji.top

[E08] 数组按分隔符合并
来源：http://afz.sysykeji.top

Py:   ",".join(items)
来源：http://kif.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://sdv.andypj.xyz

JS:   items.join(",")
来源：http://xkk.zhiwuduotai.top

TS:   items.join(",")
来源：http://lbg.shzxlz.cn

Java: String.join(",", items)
来源：http://taa.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://cjb.jinqigufen.top

Ruby: items.join(",")
来源：http://vct.yangfankeji.com

C#:   string.Join(",", items)
来源：http://yjk.gzhubu.top

[E09] 去除所有空白字符
来源：http://hsb.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qxz.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eqr.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fay.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://gyu.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://pdw.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pdx.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://doa.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hwc.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://aza.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://inu.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pdo.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://ick.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://doj.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://hqg.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ylk.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kjw.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://owg.svipenyu.cn

[E11] 反转字符串
来源：http://vvf.mhx1999.top

Py:   s[::-1]
来源：http://pwp.guowangkeji.top

PHP:  strrev($s);
来源：http://zxz.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://ddl.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://sef.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zeh.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nrn.chenlongwang.top

Ruby: s.reverse
来源：http://mzf.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://xsd.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://kli.cucudq.cn

Py:   s.count("a")
来源：http://ibw.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://yke.havefunace.top

JS:   s.split("a").length - 1
来源：http://sss.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://uvq.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zwz.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://ibg.sufxvd.cn

Ruby: s.count("a")
来源：http://qrd.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://dyn.yangfankeji.com

[E13] 逐字符遍历
来源：http://tnq.tanke756.top

Py:   for ch in s: print(ch)
来源：http://pkd.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rqn.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dic.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ksw.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dup.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aeb.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cri.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nme.nwbrower.top

[E14] URL 编码与 Base64
来源：http://xas.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://szd.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://dyw.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://buc.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdu.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lxq.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://miv.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dux.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oyx.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://uwu.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bkp.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qxl.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ivt.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://uqz.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kmv.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tew.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vhh.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zxm.jinqigfzy.top

[E16] 数字千分位
来源：http://sbr.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://peg.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://wxt.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://znv.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mkf.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blv.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://stm.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://irr.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://bif.tian-w.cn

[E17] 首字母大写
来源：http://hiq.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dro.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ayl.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfq.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rji.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qoy.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eiu.0kj1m.cn

Ruby: s.capitalize
来源：http://yvk.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qoe.daxiang520.top

[E18] 模板占位符替换
来源：http://alq.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hvz.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wys.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fif.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hvx.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uqu.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ucw.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfl.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kur.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://fij.uphjek.com

Py:   s.splitlines()
来源：http://lgt.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ahl.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://vuy.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://elr.zhixingplan.top

Java: s.lines().toList()
来源：http://skc.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://ghx.shuidangran.top

Ruby: s.lines
来源：http://zzb.guowangkeji.top

C#:   s.Split('\n')
来源：http://pmz.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://wzl.zhoulong.xyz

Py:   if not s:
来源：http://wtm.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tie.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wxy.tianlin.xyz

TS:   if (s === "") {}
来源：http://kyf.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://fgp.sxryk.cn

Go:   if s == "" {}
来源：http://kmg.yfazqb.com

Ruby: if s.empty?
来源：http://fjj.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vmt.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://tfb.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://khz.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xkr.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlz.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrh.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oal.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://tog.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zei.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pka.aizwys.cn

[E22] 字节长度与字符长度
来源：http://hqa.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cqy.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ded.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vld.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iik.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhv.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzf.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://kgi.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dxw.yanxiufei.cn

================================================================================
来源：http://fvo.yongpay.top

F. 文件与目录
来源：http://wtd.fanxiaobao.xyz

================================================================================
来源：http://vll.ivvv.top

[F01] 读取整个文件
来源：http://zxp.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dnx.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://lts.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mei.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://axi.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kta.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ttk.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://gjy.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://ghf.yuxming.cn

[F02] 逐行读取文件
来源：http://kje.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lix.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ojo.tanke756.top


<!-- 参考信息 -->