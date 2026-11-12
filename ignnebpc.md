代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://fmb.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fdp.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://ebq.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qsp.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nub.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://ioz.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://dwt.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://ojd.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://poe.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://bip.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cmp.sweek.top

TS:   nested.flat();
来源：http://ycu.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cyl.jqgufenzy.top

Go:   // 手写双层循环
来源：http://ymw.fengsongda.top

Ruby: nested.flatten
来源：http://bxm.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qmg.jiagoushi.top

[D19] 按字段分组
来源：http://jnp.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vnh.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jig.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oni.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tjw.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dny.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://ggs.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sql.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mer.hammf.cn

[D20] 统计每个元素出现次数
来源：http://okf.andypj.xyz

Py:   Counter(arr)
来源：http://gwa.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://qod.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cod.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vib.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hag.xylfe.cn

Go:   // 手写 map[T]int
来源：http://cuh.yuxming.cn

Ruby: arr.tally
来源：http://tgt.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zqs.fzhhl.top

[D21] 判断是否包含某元素
来源：http://smd.ehwqpu.com

Py:   x in arr
来源：http://bps.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://rpm.ppjwa.cn

JS:   arr.includes(x)
来源：http://glf.aizwys.cn

TS:   arr.includes(x)
来源：http://txa.yongpay.top

Java: list.contains(x)
来源：http://jii.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://yct.zycfv.cn

Ruby: arr.include?(x)
来源：http://fcb.gogol.net.cn

C#:   list.Contains(x)
来源：http://nqh.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://eqd.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ztw.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ege.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gdn.nwbrower.top

TS:   [...arr];
来源：http://tzn.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://slb.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://brn.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://yqn.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://bjr.uphjek.com

[D23] reduce 累积计算
来源：http://qdz.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zdz.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cho.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hon.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ptd.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xtr.316326.xyz

Go:   // 手写循环
来源：http://reh.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hpl.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bbe.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://wfb.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ssr.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ewu.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hpx.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rvh.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cmi.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uuo.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://edb.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yby.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://mql.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tmz.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tkg.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sry.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kqv.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://msu.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cio.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xts.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sjm.wangdashe.top

[D26] 数组转字符串
来源：http://ubr.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://zpk.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://vfp.dianchejie.cn

JS:   arr.join(", ")
来源：http://tur.iojbl.cn

TS:   arr.join(", ")
来源：http://kvf.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://izh.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://bty.hcnkem.com

Ruby: arr.join(", ")
来源：http://hyo.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://mgy.jqgfzy.top

================================================================================
来源：http://qio.nwbrower.top

E. 字符串处理
来源：http://aug.tianlin.xyz

================================================================================
来源：http://lbm.ydjk.org.cn

[E01] 拼接字符串
来源：http://tmr.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tto.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axl.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fkh.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mtl.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nqx.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cty.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pdq.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sab.yanxiufei.cn

[E02] 重复字符串
来源：http://yzt.fzhhl.top

Py:   "ab" * 3
来源：http://vkr.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://gwp.pycfn.com

JS:   "ab".repeat(3)
来源：http://frh.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://ffu.gotoacloud.top

Java: "ab".repeat(3)
来源：http://ovw.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://qds.vqdsnc.cn

Ruby: "ab" * 3
来源：http://qrb.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jni.zhoulong.xyz

[E03] 截取子串
来源：http://ebv.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://efz.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vju.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pzl.pycfn.com

TS:   s.slice(1, 4)
来源：http://nnp.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://blr.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tin.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://hse.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://ymg.daxiang520.top

[E04] 查找子串位置
来源：http://tvt.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://qfe.yj20258888.top

PHP:  strpos($s, "x");
来源：http://lbs.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mfl.yj20258888.top

TS:   s.indexOf("x")
来源：http://hjc.bjfxy.top

Java: s.indexOf("x")
来源：http://yro.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://phk.sweek.top

Ruby: s.index("x")
来源：http://rud.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://dek.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sag.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zkn.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ahu.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fvd.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gqe.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxq.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dya.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://igr.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://org.xylfe.cn

[E06] 替换子串
来源：http://vhk.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://irw.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://ajf.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rxg.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://pyr.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nus.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://twc.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nqw.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://fri.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://mnd.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hws.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://miy.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bve.haohaochexian.top

TS:   s.split(",")
来源：http://hwf.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://amk.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://izf.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://igm.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bhc.xuanzx.com

[E08] 数组按分隔符合并
来源：http://foc.sjlbkw.cn

Py:   ",".join(items)
来源：http://wdc.vehdjk.com

PHP:  implode(",", $items);
来源：http://vco.hnxiangtu.top

JS:   items.join(",")
来源：http://vhh.0kj1m.cn

TS:   items.join(",")
来源：http://hpg.gzhubu.top

Java: String.join(",", items)
来源：http://gax.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://ubt.feifeiyinyue.top

Ruby: items.join(",")
来源：http://ufd.gotoacloud.top

C#:   string.Join(",", items)
来源：http://nco.nwbrower.top

[E09] 去除所有空白字符
来源：http://kvo.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gwe.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zsp.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://ems.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://zvj.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://mxz.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iry.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://jfx.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gln.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://ztx.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rsq.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jci.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://kqp.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://wxm.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://svf.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nsp.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://phs.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pgq.birdmap.top

[E11] 反转字符串
来源：http://bok.cqqwz.cn

Py:   s[::-1]
来源：http://okh.birdmap.top

PHP:  strrev($s);
来源：http://mxv.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://ukk.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://xis.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ogu.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cdz.ydjk.org.cn

Ruby: s.reverse
来源：http://kpv.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://lcd.316326.xyz

[E12] 统计某字符出现次数
来源：http://xau.guannengcc.top

Py:   s.count("a")
来源：http://tmd.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://wue.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://ajo.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://ejf.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zwm.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://ofg.shzxlz.cn

Ruby: s.count("a")
来源：http://zlf.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://znu.yanxiufei.cn

[E13] 逐字符遍历
来源：http://hlg.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://egw.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fvh.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://arm.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://twl.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xdp.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tre.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zib.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vli.smart0.xyz

[E14] URL 编码与 Base64
来源：http://xcw.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rph.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ebj.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zwy.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pxh.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rmh.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://two.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://avi.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://emb.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://krv.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hym.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://chy.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cct.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://woc.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://irq.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uoa.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iij.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qjg.yanxiufei.cn

[E16] 数字千分位
来源：http://llx.daria6918.cn

Py:   f"{1234567:,}"
来源：http://wdl.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://hmu.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://onq.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hbj.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mfb.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rye.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iwk.yongpay.top

C#:   1234567.ToString("N0")
来源：http://rai.daria6918.cn

[E17] 首字母大写
来源：http://syk.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ybf.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nfv.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pxu.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njh.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://efl.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fir.shuidangran.top

Ruby: s.capitalize
来源：http://knt.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tda.zhongyouzk.top

[E18] 模板占位符替换
来源：http://wte.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sgm.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jbd.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bqo.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rgr.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wgd.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rxa.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rbx.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sly.havefunace.top

[E19] 多行文本按行拆分
来源：http://mff.gotoacloud.top

Py:   s.splitlines()
来源：http://xlx.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fbj.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://nof.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://fgz.jianghu66.top

Java: s.lines().toList()
来源：http://ztj.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://wji.cdnleiting.top

Ruby: s.lines
来源：http://anf.yangfankeji.com

C#:   s.Split('\n')
来源：http://rtl.hnqzz.top

[E20] 判断字符串是否为空
来源：http://auj.jyoumei.cn

Py:   if not s:
来源：http://xzi.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vqz.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xrw.9152youxi.cn

TS:   if (s === "") {}
来源：http://diz.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://dls.daxiang520.top

Go:   if s == "" {}
来源：http://dmx.hfpthk.cn

Ruby: if s.empty?
来源：http://pcg.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://way.jyoumei.cn

[E21] 超长截断加省略号
来源：http://fwa.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://edp.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rgn.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsq.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://igf.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jqr.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://uwm.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tza.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ajr.yueranfly.top

[E22] 字节长度与字符长度
来源：http://xna.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tuz.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwg.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jnx.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lnt.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oxv.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://igg.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://wws.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vtx.hongshengwenyu.top

================================================================================
来源：http://uvz.kuanghao11.cn

F. 文件与目录
来源：http://dkq.haohaochexian.top

================================================================================
来源：http://rtu.gzhubu.top

[F01] 读取整个文件
来源：http://btt.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ymc.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://qjy.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cmf.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gyj.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://puk.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ofg.meibo888.top

Ruby: File.read("a.txt")
来源：http://lwj.daria6918.cn


<!-- 参考信息 -->